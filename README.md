# KAIST CS492 Formal Modeling and Verification of Complex SW Systems (Fall'23)


## Announcement


## Administrative Information

- Instructor: [Prof. Moonzoo Kim](https://swtv.kaist.ac.kr/members/mzkim)

  - Office: 2434 (located at the east wing of E3-1)
  - Phone: 042-350-3543
  - E-mail: moonzoo.kim @ gmail.com
  - Office hour: Tues 3:00-4:00 PM (reservation e-mail is preferred)

- Teaching assistants: Ahcheong Lee (youngseok.choi@kaist.ac.kr)  

- Lecture hours: Tue/Thur 4:00 - 5:15 PM

- Lecture room: E3 Rm#1101 (and through Zoom)
  - a face-to-face lecture on Tues and an online lecture on Thurs (this plan may change later) 
  - Zoom link for Thurs class: https://kaist.zoom.us/j/5258253316
<!---
- Prerequisite: proficiency in C/C++ programming and Linux utilities
  - Due to the high load of TA, TA will not provide help for basic C/C++/Linux questions.
  - Highly recommend to take CS458 after taking CS230 System Programming first
 --->
  
- Grading: attendance/class participation/quiz: 30%, HW: 40%, final exam:40%
  - You should turn on your web cam when you participate an online class; class attendance will not be counted otherwise.
  - More than 7 absences of the class will get F grade
  - Late attendance shall be counted as 1/3 absence. If a student is not able to attend a class due to an important event (e.g., attending conf., etc.), he/she should submit 1 week prior notice to the professor.
  - The official language in the class is English. All students should submit all written documents such as homework, project reports, exam, etc. in English; 20% penalty of the max score otherwise.  

- Homework:
  - Homework should be submitted through KLMS https://klms.kaist.ac.kr/course/view.php?id=145058
  - Late HW will be accepted with 10% penalty of the max score in 1 day, 30% penalty of the max score in 3 days. HW will not be accepted after then.
    - Hint: many questions of exams are from the homeworks.
  - All programming HWs you submit must be able to be replayed by executing a single script file on a TA's server account (i.e., submitted HW should not have a dependency on your home directory, environment, etc.).  Also, the replayed execution must demonstrate the same output to the submitted hw. You will get 10% penalty of the max score otherwise.
  - For your programming HWs, you should not use external libraries which are not available on the server machines.  If you really need an external library, you have to ask TAs to install it on the server machines.
  - Please, include your student ID in the name of your submiited file(s), so that TAs can easily identify which files are yours.
  
- Questions on the course materials and homeworks should be posted as github issues 
  - https://github.com/swtv-kaist/cs458-spring23/issues 


## Syllabus
This class covers formal techniques to model and verify complex SW Systems. It is highly challenging to design and verify SW systems correctly because of the high complexity of SW systems caused by reactive characteristics, concurrency, platform dependency and so on. Students will learn formal techniques to resolve such 

systematic SW modeling and verification techniques. automated SW testing/verification techniques to detect SW bugs by analyzing **SW source code** and its **diverse runtime behaviors**. In particular, this class focuses to teach techniques that automatically generate test cases to achieve high code coverage and, thus, to detect many bugs. 

The class teaches **practical applications** of testing/verification techniques by applying open-source testing/verification tools to complete homework tasks. Also, it guides students to learn the underlying fundamental algorithms of such techniques/tools to improve the performance of automated testing/verification.

## Course Schedule

### Part I: Overview of High Complexity of SW  

- Feb 28 : [Introduction](1-overview/lec1-Intro-AutomatedSWAnalysis_v11.pptx) [[pdf]](1-overview/lec1-Intro-AutomatedSWAnalysis_v11.pdf)

<!--  Feb 28 : <a href="part2-coverage/lec1-Intro-AutomatedSWAnalysis_v11.pptx" download> Introduction2 </a> -->

- Mar 2, 7: [Necessity for systematic & automated testing techniques](1-overview/lec2-Intro-HighComplexitySW_v9.pptx) [[pdf]](1-overview/lec2-Intro-HighComplexitySW_v9.pdf)

  - "Variability and Reproducibility in Software Engineering: A Study of Four Companies that Developed the Same System" by Anda et al.
IEEE Trans. on Software Engineering vol. 35, no. 3, pp. 407-429, May-June 2009.

- Mar 9: [Overview of testing techniques (including the input partitioning technique)](1-overview/lec3-testing-overview-v3.pptx) [[pdf]](1-overview/lec3-testing-overview-v3.pdf)

### Part II: Systematic Modeling and Verification by using Process Algebra CCS

- Sep 4: Intro. to Process Algebra

- Sep 9: Formal Semantics of CCS

- Sep 11: Examples of CCS models

- Sep 23: Equivalence Semantics of CCS

- Sep 25: Case study of multiple reader/writer system

- Sep 30: Equivalence hierarchy

### Part III:  Model Checking by using SPIN and NuSMV Model Checkers
  

- Oct 9th: Computational Tree Logic

- Linear Temporal Logic

- Oct 14th: Model checking- NuSMV (1/2)

- Oct 16th: Model checking- NuSMV (2/2)

- Oct 28th: Model checking- Spin (1/3), Spin (2/3)

- Oct 30th: Spin - advanced features

- Esterel
https://stackoverflow.com/questions/50460177/signal-vs-esterel-vs-lustre

### Part IV: SAT-based Model Checking by using CBMC Model Checker

- May 16, 18: [SAT-based bounded software model checking](4-model-checking/lec21-model_checking-v3.pptx) [[pdf]](4-model-checking/lec21-model_checking-v3.pdf)
  - The importance of unwinding loop bound: SAT-based Bounded Software Model Checking for Embedded Software: A Case Study, APSEC 2014 by Kim et al

- May 23: [Software model checking examples](4-model-checking/lec22-SMC-examples-v4.pptx) [[pdf]](4-model-checking/lec22-SMC-examples-v4.pdf), [CBMC memory model](4-model-checking/lec25-cbmc-memory-model.pptx) [[pdf]](4-model-checking/lec25-cbmc-memory-model.pdf)
  - code examples for CBMC
  - cbmc-memory-model-example.zip

- May 25:  [Model Checking flash memory storage platform software - an industrial case study](4-model-checking/lec26-ase08-v2.pptx) [[pdf]](4-model-checking/lec26-ase08-v2.pdf)
  - "A Comparative Study of Software Model Checkers as Unit Testing Tools: An Industrial Case Study," IEEE Transactions on Software Engineering (TSE), vol 37, no 2, pages 146-160, March 2011
  - "Formal Verification of a Flash Memory Device Driver- an Experience Report" Spin 2008, by M.Kim, Y.Kim, Y.Choi, and H.Kim

- May 30: [Verification of the multi-sector read of flash memory storage](4-model-checking/lec27-SMC-examples2.pptx) [[pdf]](4-model-checking/lec27-SMC-examples2.pdf) 


### Part V: Testing/Verification Engine - SAT/SMT Solver

- June 1: [SMTlib tutorial](5-smt/lec40-smtlibV2-v5.pptx) [[pdf]](5-smt/lec40-smtlibV2-v5.pdf), [SMTLib web page](https://smtlib.cs.uiowa.edu/), [First order theories](5-smt/lec43-first-order-theories.pptx) [[pdf]](5-smt/lec43-first-order-theories.pdf)
  - SMTlib examples
  - Examples of First Order Theories [pdf] (for concolic testing, UML OCL, JML, pre/post condition verification, etc)
  - Definition of "theory"
  - CS402 Intro to Logic (Predicate Calculus - Semantics)
  - SMT-competition 2022

- June 8: [Using SAT solver for Sudoku](5-smt/lec44-sudoku-v2.pptx) [[pdf]](5-smt/lec44-sudoku-v2.pdf), Q&A for the final exam, LLVM IR basics, CLANG vs LLVM
  - "Sudoku as a SAT problem" by I.Lynce and J.Ouaknine, Intl. Symp. on Artificial Intelligence and Mathematics 2006
  - The SuDoku Puzzle as a Satisfiability Problem

- **June 13:  Final exam (closed book)**

