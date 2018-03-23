#### Status : In progress

# Technical-Interview

###### **Description**: This document is a definition of "Technical interview", forms of implementation, methods of application, importance and includes general advices.

###### **Note**: The material was based on my experiences based on about 100 technical interviews I conducted and feedback from applicants.
- - - -

Contents
========

* [Definition](#definition)
* [Passing methods](#passing-methods)
  * [Oral Technical Interview](#oral-technical-interview)
    * [Appropriate environment](#appropriate-environment)
    * [The correct sequence of technical questions](#the-correct-sequence-of-technical-questions)
    * [Common questions](#common-questions)
    * [The “last” question](#the-last-question)
  * [Quiz](#quiz)
  * [Task](#taks)
  * [Comparison](#comparison)
* [Importance of Technical Interview](#importance-of-technical-Interview)
* [Disclaimer](#disclaimer)

- - - -

Definition
========

The technical interview as a process pursues the following purpose:  
**to estimate applicant's technical knowledge maximum objectively  at a given time and possible potential at the upcoming time period.**
- - - -

Passing methods
========

The main techniques for conducting a technical interview are "Oral", "Test Quiz" and "Technical" task. Any method has its purpose and order  form of conduct. The above mentioned can be conducted as separate stages in different sequences orders. Depending on company requirements “Quiz” and “Technical task” may be missed. As a rule, the essential and minimal consisting part of the technical interview is the oral technical interview, and the main stages are considered the "Oral" and "Technical task".

### Oral Technical Interview

#### Appropriate Environment

Based on the above definition the main purpose of the Tech specialist is the estimation of the applicant's technical knowledge maximum objectively, that is to say, first of all, to create an appropriate environment for the applicant to be psychologically balanced, otherwise the result can not be considered an objective estimation.
In the case if the applicant is strained, this fact can have an impact on his answers and self-expression.

To create a comfortable environment.

  * It is desirable to conduct a technical interview with one or two tech. specialist, but not more [(1)](#the-count-of-interviewers).
  * Do not start immediately with technical questions. For example: 
  
      | | |
      | --- | --- |
      | **Tech. specialist** | - Hello! (smile :)) |
      | **Applicant** | - Hello! |
      | **Tech. specialist** | - My name is Jon. |
      | **Applicant** | - Pleasant, Jack. |
      | **Tech. specialist** | - It's nice Jack, how are you? |
      | **Applicant** | - Good, thanks, and how are you? |
      | **Tech. specialist** | - Good, thank you. Аre you in a good mood? |
      | **Applicant** | - In fighting mood:) |
      | **Tech. specialist** | - Ok, Jack, it will be technical interview, mostly from JavaScript, but before I go through formal inquiries, I  want some information about you, ok?. Tell a little about yourself, education, experience and more. |
      | **Applicant** | - ... |
  * Maximally avoid denying the applicant's thoughts during the interview (**"You are wrong"**, **"The claim was not correct"**, etc.). At the end of the interview you can go through all his mistakes, give advice etc, if the applicant wishes. (2). At the same time, the interview should not present one-sided questions. For example:  
      
      | | |
      | --- | --- |
      | **Tech. specialist** | - Please provide JavaScript as a programming language, in some sentences in your own words,  as you are comfortable. |
      | **Applicant** | - Well, Javascript is a scripting language, faster, used in the browser as well as on BackEnd, etc. |
      
      The answer above is inaccurate, insufficient from the technical aspect. Desirable, relatively more professional and anticipated answer could be the following:  
      
      &#45; JavaScript is a multi-paradigm, interpreted, single threaded and dynamic typed programming language.
      
      The difference between the applicant's answer and the supposed correct answer is still insufficient to suppose that the applicant does not know about such ideas as "multi-paradigm'', ''interpreted'', ''single threaded'', ''dynamic typed'', etc. The next question.  
      
      &#45; Look, almost all the programming languages have common characteristics, they are - dynamic or static? Single threaded or multi threaded? Interpreted or compiled? etc. Let's try to answer to the following questions considering as a target of the conversation JavaScript. Let's start from the first question - dynamic or static?  
      
#### The correct sequence of technical questions

The correct sequence of technical questions (from the perspective of complexity) enables accurate assessment of the applicant's knowledge. Usually a problem arises not about knowing whether the applicant knows or does not know the problem, but how many percent knows. In such cases it is necessary to be able to accurately estimate the percentage ratio for which the issues relating to the problem should be arranged in terms of ascending complexity, and the starting point or the next step of the transition is determined from the applicant's technical level (junior, middle, senior, etc.).

Often encountered problem:  
usually, a lower-level specialist is given a "sophisticated" question without answering to it, the applicant's knowledge of the given problem may be estimated to 0, whereas the applicant had some understanding and knowledge about the problem.  

To illustrate the organization of correct sequence of technical questions, we should divide questions into two groups:

  1. Questions related to the concrete topic and classification of these questions by complexity.  
    
      Example (as an example will be considered setTimeout from WebAPIs).  
      Possible questions related to setTimeout in the correct order. 

      | | |
      | --- | --- |
      | 1 | - Describe setTimeout as a function.<br/>* Not important questions: <br/>1. Can the first argument of setTimeout not be a function? <br/>2. is there a third argument for setTimeout, if yes what does it represent and has it limitations, if yes, then what kind of limitations? |
      | 2 | - Give a mathematical claim for the second argument of setTimeout. |
      | 3 | - Detailed description of setTimeout's work. |
      | 4 | - Recursive setTimeout and setInterval. |
      | 5 | - setTimeout (fn, 0) as an exception. |
      | 6 | - Dom minimum timeout value. |
      | 7 | - setImmediate, setImmediate 's polyfill, polyfill implementation.<br /> * postMessage <br /> * messageChannel <br /> * <script> onreadystatechange |
      | 8 | - process.nextTick, Promise.resolve(). Compare with setTimeout() |
      | 9 | - Task, MicroTask, differences, execution order, implementation in different browsers. |
      | 10 | - setTimeouts’ execution order - FIFO, LIFO, random |

      If we do not set the correct sequence, and then start talking about setTimeout starting with Question 6 or its specific case, for example:  
      &#45; Please enter DOM_MIN_TIMEOUT_VALUE or DOM_CLAMP_TIMEOUT_NESTING_LEVEL in Google Chrome and FireFox?  
      then the wrong answer to the question or the lack of a response can not give any information about the applicant's setTimeout knowledge.  

      **Use the right sequence of questions.**
  
  2. Topics that you can address only if the applicant is in line with that level.  
  
      Example - Questions related with engine.  
      
      * Parsing
        * Lazy Parsing
          * Pre parsing
          * Full parsing
      * Tockenazing/Lexing
      * AST ( Abstract Syntax Tree )
      * JIT (Just in Time compiler)
        * Compile + Optimization
        * Re-optimization / De-optimization
      * Automate Memory Management - GC
        * Comparison with manual memory management
        * advantages / disadvantages
      * Web Assemble
        * toolchain
          * emscripten
          * clang
          * llvm
        * Detailed description of webassembly work.
      * etc.
      
#### Common questions

The main questions are given separately (before or after) from the questions of the observed position, can also be held as a separate stage. The common questions, in their turn, are divided into two groups.

1. Common IT development questions.  

    * Algorithms theory
      * Turing machine
      * Finite-state machine (FSM), Finite-state automata (FSA), Finite automation
      * "Divide and Conquer"
      * Sorting algorithms
      * ...
    * Operating systems
    * Graph theory
      * Graph
      * Tree
      * Search algorithms
        * DFS - Depth-first search
        * BFS - Breadth-first search
      * Shortest path
      * Minimum spanning tree
      * ...
    * Data structure
      * Queue
      * Stack
      * List
      * B-tree
      * ...
    * Data bases
    * Probability theory
    * Theory of Games
    * Discrete mathematics
    * Functional programming basics
    * Classifications / Forecasting and prediction algorithms - Machine learning

    **Note:** * This questionnaire can be changed depending on company requirements, observable position and technical level of the applicant.

... to be continued
  

  
  
