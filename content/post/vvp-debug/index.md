---
title: How to find combinational logic loops in iverilog/vvp?


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

It is possible that vvp simulations get stuck and never finish. This post is about why the problem is happening and what you can do to fix it.

**Why it Happens**

The simple answer is that two of your `always @(*)` blocks are continuously triggering each other and the simulator cannot move forward.
In other words, you have _combinational logic loop_ in your design. Suppose you have two always blocks:

```verilog
reg x;
reg y;
always @(*) begin
  x = y;
end

always @(*) begin
  y = x;
end
```

Do you see what the problem is here? Every time the first always block runs, it triggers the second always block to run, and every time the second always block runs, it triggers the first always block to run. (Remember, `always @(*)` means that every time you write to one of the inputs, the whole block reruns.) Therefore, the simulator gets stuck going back and forth between the loops until eternity. Even if the logic does eventually settle (i.e. is no longer changing) as in this example, the simulator has no way of knowing that.


**Fixing the problem**

Generally speaking, combinational logic loops should be avoided. So do some analysis and make a list of all the dependencies of each of your `always @(*)` blocks, and see if you have two blocks with interlinked inputs/outputs i.e. one block writes to an output that another block reads and that other block writes to an output that the first block reads. 

**How to trace which blocks are causing the problem**

If you are having trouble discovering which two (or more) `always @(*)` blocks are the problem, try using `-pfileline=1` in your command arguments to iverilog. Then when you run vvp again, it will display which line of the code is being simulated at any given time. If there is an infinite loop, it will show you which lines are looping over and over, and this should tell you which blocks are causing the problem!

**An Alternative Approach**

If you can get the Verilog into Yosys, you may use the `scc` command in Yosys to find combinational logic loops.
