---
title: Synthesizable Verilog Coding Style


# Date published
date: "2021-08-27"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

math: true
diagram: true
highlight: true

---

(Credit to Justin Patel)


1.  **Use the**  `always @(*)`  **block for combinational logic only.** The reg types that you assign to in an `always @(*)` block are simply wires driven by the output of combinational logic blocks (i.e. although declared as `reg` in Verilog, they are coerced to behave like wires and will be synthesized as wires.
2.  **Do not assign to registers** (i.e. `assign var_register = value`) **in an** `always @(*)` **block.** 

3.  **Use the** `always @(posedge clk)` **block for sequential logic only** when you mean to create an edge-triggered register.
4.  The edge-triggered registers should be implemented using the `reg` type and assignment to these registers should be performed in one sequential block in the datatype, i.e. `always @(posedge clk)`. **Do not attempt to assign to an element that is not meant to be edge-triggered within an** `always @(posedge clk)` **block. Instead, reg types that are meant to be coerced and synthesized as wires should be in an** `always @(*)` **block.**
    
5.  **If you assign to a reg in one always block, do not assign to it in another `always` block.** All reg types should be either combinational logic outputs, which must be produced from a single `always @(*) `block, or edge-triggered registers, which should be assigned to in a single `always @(posedge clk)` block.
6.  **Within an** `always @(*)` **block, use ONLY blocking assignment (**`=`**).**
7.  **Within an** `always @(posedge clk)` **block, use ONLY non-blocking assignment (**`<=`**).**
8.  **Set a default value for each signal you assign to within an** `always @(*)` **block.** For every signal that is assigned to within an `always @(*)` block, you should set a default value at the top of the block before any other logic. This is done to avoid implicit latching. You can sometimes get away without it (if the signal is assigned to in all possible branches), but doing it anyways ensures you won't see certain errors. For example:   
    
    ```verilog
    reg x;
    always @( * ) begin
        x = 0; // default value
    
        // other logic
        if (y) begin
            x = z;
        end
    end
    ```
    
9.  **Ensure that each register assigned to within an** `always @(posedge clk)` **block is assigned to only once.** This is different from an `always @(*)` block, where you may (and probably should) assign to a variable multiple times during one execution of a block. To ensure this, it is recommended that the assignments to the same register are grouped to a if-else-if-...-else statement, for example:  
    
    ```verilog
    reg[5:0] count;
    always @(posedge clk) begin
       if(count_clear)
           count <= 0;
       else if(count_inc)
           count <= count + 1;
       else if(count_dec)
           count <= count + 1;
     // maybe you don't need the else-statement
     // it is the same as having
     // else 
     //    count <= count;
    ```
    
10.  For the testbench, for the wires that are connected to the output of the module-under-test, they should **not** be assigned an initial value.
    

```
// in Testbench
module SimonDatapathTest;

reg [3:0] pattern;  // this should be reg, because it feeds the input
wire pattern_legal; // this should be wire, and NOTE: do not assign any value here !!! 
                    !
SimonDatapath dpath (
  .clk  (clk),
  .pattern(pattern),  // this is the input
  // ...
  .pattern_legal(pattern_legal), // this is the output
  // ...
);
```
