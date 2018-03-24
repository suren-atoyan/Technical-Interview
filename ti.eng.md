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
  * [Task](#task)
  * [Comparison](#comparison)
* [Importance of Technical Interview](#importance-of-technical-interview)
* [Disclaimer](#disclaimer)
* [Notes](#notes)

- - - -

Definition
========

The technical interview as a process pursues the following purpose:  
**to estimate applicant's technical knowledge maximum objectively  at a given time and possible potential at the upcoming time period.**
- - - -

Passing methods
========

The main techniques for conducting a technical interview are "Oral", "Test Quiz" and "Technical Task". Any method has its purpose and order  form of conduct. The above mentioned can be conducted as separate stages in different sequences orders. Depending on company requirements “Test Quiz” and “Technical Task” may be missed. As a rule, the essential and minimal consisting part of the technical interview is the oral technical interview, and the main stages are considered the "Oral" and "Technical Task".

### Oral Technical Interview

#### Appropriate Environment

Based on the above definition the main purpose of the tech. specialist is the estimation of the applicant's technical knowledge maximum objectively, that is to say, first of all, to create an appropriate environment for the applicant to be psychologically balanced, otherwise the result can not be considered an objective estimation.
In the case if the applicant is strained, this fact can have an impact on his answers and self-expression.

To create a comfortable environment.

  * It is desirable to conduct a technical interview with one or two tech. specialist, but not more [(1)](#note-1).
  * Do not start immediately with technical questions. <details> <summary>For example: </summary>
  
      | | |
      | --- | --- |
      | **Tech. specialist** | - Hello! (smile :slightly_smiling_face:) |
      | **Applicant** | - Hello! |
      | **Tech. specialist** | - My name is John. |
      | **Applicant** | - Pleasant, Jack. |
      | **Tech. specialist** | - It's nice Jack, how are you? |
      | **Applicant** | - Good, thanks, and how are you? |
      | **Tech. specialist** | - Good, thank you. Аre you in a good mood? |
      | **Applicant** | - In fighting mood:) |
      | **Tech. specialist** | - Ok, Jack, it will be technical interview, mostly from JavaScript, but before I go through formal inquiries, I  want some information about you, ok? Tell a little about yourself, education, experience and more. |
      | **Applicant** | - ... |
      
      </details>
  * Maximally avoid denying the applicant's thoughts during the interview (**"You are wrong"**, **"The claim was not correct"**, etc.). At the end of the interview you can go through all his mistakes, give advice etc, if the applicant wishes. [(2)](#note-2). At the same time, the interview should not present one-sided questions. For example:  
      
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
      | 1 | - Describe setTimeout as a function.<br/>* Not important questions: <br/>1. Can the first argument of setTimeout not be a function? <br/>2. Is there a third argument for setTimeout, if yes what does it represent and has it limitations, if yes, then what kind of limitations? |
      | 2 | - Give a mathematical claim for the second argument of setTimeout. |
      | 3 | - Detailed description of setTimeout's work. |
      | 4 | - Recursive setTimeout and setInterval. |
      | 5 | - setTimeout (fn, 0) as an exception. |
      | 6 | - Dom minimum timeout value. |
      | 7 | - setImmediate, setImmediate 's polyfill, polyfill implementation.<br /> * postMessage <br /> * messageChannel <br /> * <script> onreadystatechange |
      | 8 | - process.nextTick, Promise.resolve(). Compare with setTimeout() |
      | 9 | - Task, MicroTask, differences, execution order, implementation in different browsers. |
      | 10 | - setTimeouts’ execution order - FIFO, LIFO, random |

      Let's consider that we do not set the correct sequence, and then start talking about setTimeout starting with Question 6 or its specific case, for example:  
       &#45; Please enter DOM_MIN_TIMEOUT_VALUE or DOM_CLAMP_TIMEOUT_NESTING_LEVEL in Google Chrome and FireFox.  
      In that case the wrong answer to the question or the lack of a response can not give any information about the applicant's setTimeout knowledge.  

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

    * Algorithms Theory
      * Turing Machine
      * Finite-State Machine (FSM), Finite-State Automata (FSA), Finite Automation
      * "Divide and Conquer"
      * Sorting Algorithms
      * ...
    * Operating Systems
    * Graph Theory
      * Graph
      * Tree
      * Search Algorithms
        * DFS - Depth-First Search
        * BFS - Breadth-First Search
      * Shortest Path
      * Minimum Spanning Tree
      * ...
    * Data Structure
      * Queue
      * Stack
      * List
      * B-tree
      * ...
    * Data Bases
    * Probability Theory
    * Theory of Games
    * Discrete Mathematics
    * Functional Programming Basics
    * Classifications / Forecasting and Prediction Algorithms - Machine Learning

    **Note:** * This questionnaire can be changed depending on company requirements, observable position and technical level of the applicant.
    
2. Questions related to the applicant's IT preferences

    | | |
    | --- | --- |
    | 1 | - Preferred Operating system |
    | 2 | - Preferred text editor or IDE |
    | 3 | - In addition to your basic programming language mention other languages you are interested in or want to work on? |
    | 4 | - How do you follow news? What resources do you use? |
    | 5 | - For what goals does your GitHub account serve (if you have any)? |  
    
    **Note:** Any question of this questionnaire as a separate question may not provide sufficient information about the applicant. However, the answer to all questions, as a whole, may allow to understand the applicant’s world outlook in IT. For example: let’s review the answers of two different applicants.  
    
    Option 1.  
    
    | | |
    | --- | --- |
    | 1 | - Windows |
    | 2 | - Microsoft Visual Studio, WebStorm, Notepad++ |
    | 3 | - C#, Visual Basic, PHP |
    | 4 | - Looking for Google on what I need. I read Toster.ru and, in general, look at screencasts on Youtube.com |

    Option 2.  
    
    | | |
    | --- | --- |
    | 1 | - Linux, Unix-like operating systems. |
    | 2 | - Vim, Sublime Text or other text editor, but not IDE |
    | 3 | - C/C++, Rust, OCaml, Elixir (Erlang/OPT), Python |
    | 4 | - Medium, Hackernoon, Habr, Twitter... I am subscribed to Google’s and Mozilla's Youtube channels |

    Note ... * Examples are from real life.  
    
#### The "last" question

**- Please rate your technical knowledge in the 0 to 10 point system.**

During the interview, the tech. specialist will be forming an assessment that will be considered an alleged objective assessment and it is also important to get that assessment by the applicant. And from the comparison of the two estimates additional assumptions may be made.

### Task

The technical task presents technical issue representation corresponding to the position observed. The purpose of this method is to evaluate the applicant's technical knowledge from the point of view of the practical tasks implementation.  
They can be:

* Code quality
* Coding style
* Code architecture
* Naming convention
* File/Folder structure
* ...

##### Important points

* The estimation of the problem should be left to the applicant's discretion. The assessment of the complexity of his problem and the time/quality ratio may serve as additional information.
* The complexity of the task is not the main goal, and is mainly lower than the applicant's technical level.
* Task responses are desirable to be checked by several technical experts for a more objective assessment.
* The task must have a functional and technical specification and requirements.

### Quiz

Quiz or test work is a sequence of questions with possible answers. This method can be used for filtration of the preceding stages or as additional information in the main stages.

### Comparison

* Quiz
 * Advantage  
   Minor effort.
 * Disadvantage  
   Answering frequently asked questions and lacking oral conversation may be not an objective assessment.
* Task
 * Advantage  
   Opportunity to evaluate practical work.
 * Disadvantage  
   Usually, "technical work" is made remote, and lack of control and the availability of side-by-side assistance affects the validity of the work evaluation.
* Oral
 * Advantage  
   An objective assessment of theoretical knowledge, existence of oral conversation.
 * Disadvantage  
   In some cases, it is difficult to evaluate the applicant's knowledge of his or her oral speech or self-reported problems.

- - - -

Importance of Technical Interview
========

Any technical interviewing course unequivocally shows the technical level of the company.  
<br />
Based on the assessment of the interviewer, the company may employ the applicant. An incorrect assessment of the interviewer may cause problems later on.

- - - -

Disclaimer
========

The document does not aim to compile an ordered process of technical interview or passing phases for specific programming language, technology or company. The above mentioned points are the main clauses for technical interviews in IT, and JavaScript is just an example. (For more detailed JavaScript questionnaire as an interview guide refer the following file): The author did not try to define the stages of technical interview for keeping the document flexibility. The number and sequence of interview stages may vary depending on the programming language, the technology, the applicant's technical level, the company's requirements and resources. The above mentioned points will be considered as accurate also for interviews related to specific libraries or frameworks. For example:  

JavaScript - ReactJs / NodeJs and etc.  
Python - Django and etc.  
Rust - Exonum and etc.  
...


- - - -

Notes
========

###### Note 1

The presence  of more than two tech․ specialist in the room (in which the interview will be conducted) can create an overwhelming atmosphere. The presence of a second tech. specialist is desirable for making more objective opinion. However, if tech. specialist is experienced and can conduct the interview alone, then the presence of one tech. specialist will be more optimal.

###### Note 2

At the end of the interview, regardless of the applicant's assessment or his / her potential mentor, give 5 minutes for the consultation, note the mistakes, give advice, guide and show the gaps in the technical knowledge. Send relevant links to articles, books or other resources to fill in the gap. (Make the world a little better :slightly_smiling_face:)

Thank you.
- - - -
