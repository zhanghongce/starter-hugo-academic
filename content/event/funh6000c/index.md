---
title: MICS6000A Automated Reasoning in Electronic System Verification

#event: Courses
#event_url: https://example.org

location: Online
address:
  street: 
  city: 
  region: 
  postcode: 
  country: 

summary: In the lecture, we will discuss the application of automated reasoning techniques in the verification of software and hardware components in electronic systems. This course will cover basic knowledge on logic, Satisfiability solvers, model checking and their applications. To cultivate interactive-learning, this course also includes seminars that promote discussions and serve as extensions to the lectures. Enrolled students are required to sign up for the presentations in the seminars.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2022-02-07T10:30:00Z"
date_end: "2022-05-11T11:50:00Z"
#all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false


links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---



-----------------------


## **Please refer to Canvas as the information below could be outdated.**

-----------------------


### Logistics

  * Lecture: Online, Monday, Wednesday 10:30 AM-11:50 AM

  * Instructor: Hongce Zhang (e-mail: hongcezh AT ust DOT hk)
  * Office Hours: Friday 3-4:30 pm (please e-mail me in advance and I will send you the Zoom link)



### Schedule (Tentative)

  We will try to follow the posted schedule below. However, as it is the first time I teach this course, changes are likely.


| Week | Date    | Lecture  | Seminar  |
|------|---------|----|---|
1  | Feb 7, Feb 9   | Introduction, Propositional Logic  |     |
2  | Feb 14, Feb 16 | First Order Logic                  | Survey of hardware and software vulnerabilities |    PS1 out
3  | Feb 21, Feb 23 | SAT solvers                        |     |
4  | Feb 28, Mar 2  | SMT solvers                        | SAT solver: extensions and applications |
5  | Mar 7, Mar 9   | Temporal Logic                    | SMT solver: Nelson-Oppen |
6  | Mar 14, Mar 16 | Symbolic model checking            |     |
7  | Mar 21, Mar 23 | SAT-based model checking           |   |
8  | Mar 28, Mar 30 | Hoare Logic                        | SAT application: logic equivalence checking |
9  | Apr 4, Apr 6   | Predicate abstraction              | Model checking applications (TA tutorial session) |
10 | Apr 11         | Abstraction and Refinement  |     |
11 | Apr 20         |  |  Hot topic: neural network verification|
12 | Apr 25, Apr 27 | Concolic testing, Syntax-Guided Synthesis   |     |
13 | May 4          |                                    | Abstraction in verification, security verification  |
14 | May 11         |                                    | Final project presentation |   


### Grading


* Participation in seminars    : 20%
* Problem sets                 : 30%
* Projects                     : 30%
* Final exam                   : 20%



### Resources


 * Textbook: _The Calculus of Computation: Decision Procedures with Applications to Verification_ (by Aaron R. Bradley and Zohar Manna). [Electronic version](http://link.springer.com/book/10.1007%2F978-3-540-74113-8).
 We will use the "Foundations" part of the book.

 * Reference book: _Handbook of Model Checking_. [Electronic version](https://link.springer.com/book/10.1007/978-3-319-10575-8). This book serves as a good supplement on the algorithmic discussion.

 * Reference papers:
    - __SAT:__ Joao Marques-Silva, Ines Lynce, and Sharad Malik. Conflict-Driven Clause Learning SAT Solvers. Handbook of Satisfiability, Chapter 4, 2008. 
    - __SMT:__ Leonardo de Moura and Nikolaj Bjorner. Satisfiability Modulo Theories: Introduction and Applications. Communications of the ACM, vol. 54, no. 9, 2011. 
    - __BDD:__ Randal E. Bryant. Graph-based algorithms for Boolean function manipulation. IEEE Transactions on Computers, 100 (8), 677-691, 1986.
    - __Temporal Logic and BDD-based Model Checking:__ E. M. Clarke, E. A. Emerson, and A. P. Sistla. Automatic verification of finite-state concurrent systems using temporal logic specifications. ACM Transactions on Programming Languages and Systems, 8, 2 (April 1986), 244-263. 
    - __BMC:__ Armin Biere, Alessandro Cimatti, Edmund M. Clarke, Yunshan Zhu. Symbolic Model Checking without BDDs. In Proceedings of Tools and Algorithms for Construction and Analysis of Systems (TACAS) Conference 1999: 193-207.
    - __PDR:__ Niklas Een, Alan Mishchenko, Robert Brayton. Efficient Implementation of Property Directed
Reachability. In Proceedings of Formal Methods in Computer-Aided Verification (FMCAD) Conference 2011: 125-134.
    - __Hoare Logic:__ C. A. R. Hoare. An axiomatic basis for computer programming. Communications of the ACM 12, 10, 576-580, 1969. 
    - __Software Model Checking:__ Ranjit Jhala and Rupak Majumdar. Software model checking. ACM Computing Surveys 41, 4, Article 21, 2009. 
    - __SyGuS:__  Rajeev Alur, Rastislav Bodík, and others. Syntax-guided synthesis. In Proceedings of FMCAD 2013: 1-8. 

### Readings suggested for seminars

  Below are simply suggestions. You may pick your favourite instead.


  * Survey of hardware and software vulnerabilities
    - Binary Exploitation - Buffer Overflow Explained in Detail [Link](https://0xrick.github.io/binary-exploitation/bof1/)
    - Survey of Transient Execution Attacks and Their Mitigations [Link](https://dl.acm.org/doi/10.1145/3442479)


  * SAT solver: extensions and applications
    - A comparison of encodings for cardinality constraints in a SAT solver. [Link](https://arxiv.org/abs/1810.12975)


  * SMT solver: Nelson-Oppen
    - Chapter 10.1 _Combining Decision Procedures_ and 10.2 _Nelson-Oppen Method: Nondeterministic Version_ of [The Calculus of Computation](http://link.springer.com/book/10.1007%2F978-3-540-74113-8).


  * SAT application: logic equivalence checking
    - Improvements to Combinational Equivalence Checking [Link](https://dl.acm.org/doi/10.1145/1233501.1233679)


  * Model checking applications (TA will give the tutorial)
    - A Tool for Checking ANSI-C Programs [Link](https://link.springer.com/chapter/10.1007/978-3-540-24730-2_15)
    - [CBMC tutorial](https://www.cprover.org/cprover-manual/cbmc/tutorial/)
    - [SymbiYosys tutorial](https://symbiyosys.readthedocs.io/en/latest/quickstart.html)


  * Hot topic: neural network verification
    - Towards Proving the Adversarial Robustness of Deep Neural Networks [Link](https://arxiv.org/abs/1709.02802)

  * Abstraction in verification
    - Abstraction Mechanisms for Hardware Verification [Link](https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-106.pdf)


  * Security verification
    - Survey of Approaches for Security Verification of Hardware/Software Systems [Link](https://eprint.iacr.org/2016/846.pdf)