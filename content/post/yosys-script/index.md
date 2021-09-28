---
title: How to convert Verilog to btor2 or aiger format


# Date published
date: "2021-09-28"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

math: true
diagram: true
highlight: true

---

For your reference, below are the scripts I used for `yosys`.


## Verilog to Btor2:

```
read_verilog -formal <verilog-file>
prep -top <top-module>
flatten
memory -nomap
hierarchy -check
setundef -undriven -init -expose
sim -clock <clock-name> -reset <reset-name> -rstlen <reset-cycle> -n <simulation-cycle> -w <top-module>
write_btor  -s <btor-name>

```

For `memory` command, use `memory -nomap` if you want to keep array sort in Btor2, otherwise, use `memory` or `memory -nordff` to "word-blast" Verilog array.

## Verilog to AIGER


```
read_verilog -formal <verilog-file>
prep -top <top-module>
flatten
memory -nordff
setundef -undriven -init -expose
sim -clock <clock-name> -reset <reset-name> -rstlen <reset-cycle> -n <simulation-cycle> -w <top-module>
techmap
abc -fast -g AND
write_aiger -zinit <aiger-file>
```

