---
title: MICS6000H Logic Design Automation of Digital Systems

#event: Courses
#event_url: https://example.org

location: Rm 103, E1 Computational Labs (mixed-mode)
address:
  street: 
  city: 
  region: 
  postcode: 
  country: 

summary: Logic design and physical design are two major steps in the digital design process. This course is an introduction to the automation techniques in the logic design step. It covers the workflow from hardware description languages to gate-level netlists. In this course, we will discuss the theoretic foundations, including the basics of automata theory, lexing, parsing, synthesis and minimization of two-level and multi-level circuits, finite-state machine synthesis and verification, technology mapping, automatic test generation and timing analysis. This course, for the first time, connects frontend techniques of compilers with the introduction of logic synthesis. Compiling techniques and digital logic were typically taught in two separate courses. The combination in this course is intended to provide a more comprehensive view of the underlying techniques of modern logic design automation tools. 

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2022-09-07T09:00:00Z"
date_end: "2022-12-07T11:50:00Z"
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

  * Lecture: Wednesday 9:00 AM-11:50 AM, E1-L1-S4 Rm 103

  * Instructor: Hongce Zhang (e-mail: hongcezh AT ust DOT hk)
  * Office Hours: Friday 4:00-5:30 pm, Rm C8-5F-W2-3


### TA
  
  * Guangyu HU (ghuae AT connect DOT ust DOT hk).


### Prerequisites

  * ELEC2200: Digital Circuits and Systems (or equivalent)
  * COMP171: Data Structures and Algorithm (or equivalent)


### Schedule (Tentative)

  We will try to follow the posted schedule below. However, as it is the first time I teach this course, changes are likely.


| Week | Date    | Lecture  | Presentations  |
|------|---------|----|---|
1  | Sep 7  | Introduction  |     |
2  | Sep 14 | Lexing (I)                  |  |   
3  | Sep 21 | Lexing (II), parsing (I)   |     |
4  | Sep 28 | Parsing (II)                        |  |
5  | Oct 12 | Parsing (III),  intermediate representations  | (GTA) |
6  | Oct 19 | 2-level synthesis and minimization             | (1)(2)(3)(4)   |
7  | Oct 26 | Finite-state machine synthesis and minimization   |  (5)(6)(7)  |
8  | Nov 2  | Multi-level synthesis and minimization  |  (8)(9)(10) |
9  | Nov 9  | Technology mapping, testing, design-for-test | (11)(12) |
10 | Nov 16 | Timing analysis |  (13) |
11 | Nov 23 | Functional verification | |
12 | Nov 30 | Guest lecture & student presentation  |     |
13 | Dec 7 |  Final project presentation    |   |

### A Note on the Teaching Mode

In this course, we will practice the flipped-classroom teaching pedagogy. In the first half when we are on the compiler frontend, the instructor will give lectures and students will be the audience. This is still the traditional mode of teaching and is intended to leave the students some time to transfer into the active-learning mode. For the second half (the logic synthesis), enrolled students are expected to read the references before class and then make presentations in class to demonstrate what they have learned.


### Grading


* Presentation                 : 20%
* Problem sets                 : 30%
* Projects                     : 30%
* Final exam (online)          : 20%



### Resources

 * Textbook 1 __[Aho]__: _Compilers: Principles, Techniques, and Tools_ (by A. Aho, M. Lam, R. Sethi & J. Ullman). (This is also known as "the dragon book" because of the dragon on the front cover).
 We will only use the frontend part of this book.

 * Textbook 2 ____[Hachtel]____: _Logic Synthesis and Verification Algorithms_ (by G. Hachtel & F. Somenzi). 

 * Reference book 1 __[Kohavi]__: _Switching and Finite Automata Theory_ (by Z. Kohavi & N. K. Jha)
 * Reference book 2 __[Wang]__: _Electronic Design Automation: Synthesis, Verification, and Test_ (by L-T. Wang, Y-W. Chang & K-T. Cheng).


 * Similar courses taught around the world (so you can also learn from other sources):
    - Compilers: 
      - [Stanford CS143](https://web.stanford.edu/class/cs143/)
      - [Princeton COS320](https://www.cs.princeton.edu/courses/archive/spring20/cos320/)
      - [Cornell CS 4120/4121/5120/5121](https://www.cs.cornell.edu/courses/cs4120/2021sp/)
    - Logic Synthesis:
      - [UT Austin: ACES 6.120](http://users.ece.utexas.edu/~adnan/syn-07/)
      - [NTHU Taiwan CS 613200](http://www.cs.nthu.edu.tw/~tingting/course1.html)


### Projects

There will be two projects in this course. The first project is about lexing & parsing and the second project is about logic synthesis. The two projects are connected so that you should be able to implement a tiny toy logic synthesizer in the end.

### Topics of Presentations

Students should take turn to present the algorithms (the presentation sign-up sheet is on Canvas). Depending on the number of students actually enrolled, there could be more than one round of presentation. The suggested topics of the presentations are:

| Number | Topic    | Reference |
|------|---------|-----|
(1) | Tabular Method of Computing Prime Implicants | __[Hachtel]__ Section 4.4-4.5
(2) | Prime Implicant Selection | __[Hachtel]__ Section 4.7-4.8
(3) | Branch-and-Bound Algorithm for Unate Covering Problems |  __[Hachtel]__ Section 4.9
(4) | Heuristic Minimization of Two-Level Circuits |  __[Hachtel]__ Section 5.1
(5) | FSM State Minimization |  __[Hachtel]__ Section 7.4
(6) | FSM State Encoding Problem | __[Hachtel]__ Section 8.3
(7) | FSM Decomposition  |  __[Hachtel]__ Section 8.4
(8) | Kernels and Co-Kernels |  __[Hachtel]__ Section 10.5
(9) | Heuristic Factoring Algorithm |  __[Hachtel]__ Section 10.6
(10) | Boolean Factoring and Decomposition of Logic Networks |  Alan Mishchenko, Robert Brayton, and Satrajit Chatterjee. ICCAD 2008. (This is the fundamental of Berkeley-ABC.)
(11) | Tree-based covering: an example of algorithms for technology mapping |  __[Kohavi]__ Section 6.2
(12) | The D-Algorithm (an example of ATPG algorithms) |  __[Wang]__ Section 14.4.3
(13) | Functional Timing Analysis |  __[Wang]__ Section 6.5.2

If you are interested, there are also some advanced topics on the intersection of machine-learning and logic synthesis (we might not have time to get to these in class):

1. DRiLLS: Deep Reinforcement Learning for Logic Synthesis (2020 ASP-DAC)
2. Logic Synthesis Meets Machine Learning: Trading Exactness for Generalization (2021 DATE)

