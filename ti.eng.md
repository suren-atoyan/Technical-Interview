# Technical-Interview

###### **Description**: This document is a definition of "Technical interview", forms of implementation, methods of application, importance and includes general advice.

###### **Note**: The material is formed based on my experience of more than 150 technical interviews I have conducted and on feedback from applicants.
- - - -

Contents
========

* [Definition](#definition)
* [Interviewing methods](#interviewing-methods)
  * [Oral Technical Interview](#oral-technical-interview)
    * [Appropriate environment](#appropriate-environment)
    * [The correct sequence of technical questions](#the-correct-sequence-of-technical-questions)
    * [Common questions](#common-questions)
    * [The “last” question](#the-last-question)
  * [Quiz](#quiz)
  * [Task](#task)
  * [Comparison](#comparison)
* [The importance of Technical Interview](#the-importance-of-technical-interview)
* [Disclaimer](#disclaimer)
* [Notes](#notes)

- - - -

Definition
========

The technical interview as a process pursues the following purpose:  
**To estimate applicant's technical knowledge maximum objectively  at a given time and possible potential at the upcoming time period.**
- - - -

Interviewing methods
========

The main techniques for conducting a technical interview are "Oral", "Test Quiz" and "Technical Task". Each method has its purpose and order form of conduct. The above mentioned can be conducted as separate stages in different orders. Depending on company requirements “Test Quiz” and “Technical Task” may be missed.  
The main stages are considered the "Oral" method, which is as a rule essential and minimal consisting part of the interview and "Technical Task".

### Oral Technical Interview

#### Appropriate Environment

Based on the above definition the main purpose of the tech. specialist is the estimation of the applicant's technical knowledge maximum objectively, that is to say, first of all, to create an appropriate environment for the applicant to be psychologically balanced, otherwise the result can not be considered an objective estimation.
Applicant's tension can have an impact on his answers and self-expression.

To create a comfortable environment.

  * It is desirable to conduct a technical interview with one or two tech. specialist, but not more [(1)](#note-1).
  * Do not immediately start with technical questions. <details> <summary>For example: </summary>
  
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
  * Maximally avoid denying the applicant's thoughts during the interview (**"You are wrong"**, **"The claim was not correct"**, etc.). At the end of the interview you can go through all his mistakes, give advice, etc, if the applicant wishes. [(2)](#note-2). At the same time, the interview should not present one-sided questions. For example:  
      
      | | |
      | --- | --- |
      | **Tech. specialist** | - Please introduce JavaScript as a programming language in your own words |
      | **Applicant** | - Well, Javascript is a scripting language, faster, used in the browser as well as on BackEnd, etc. |
      
      The answer above is inaccurate, insufficient from the technical aspect. Desirable, relatively more professional and anticipated answer could be the following:  
      
      &#45; JavaScript is a multi-paradigm, interpreted, single threaded and dynamic typed programming language.
      
      The difference between the applicant's answer and the supposed correct answer is still insufficient to suppose that the applicant does not know about such ideas as "multi-paradigm'', ''interpreted'', ''single threaded'', ''dynamic typed'', etc. The next question:  
      
      &#45; Look, almost all the programming languages have common characteristics: are they dynamic or static, single threaded or multi threaded, interpreted or compiled, etc? Let's try to answer the following questions considering JavaScript as the target of the conversation. Let's start from the first question - dynamic or static?  
      
#### The correct sequence of technical questions

The correct sequence of technical questions (from the perspective of complexity) enables accurate assessment of the applicant's knowledge. Usually a problem arises not learning whether the applicant knows or doesn't know the given problem, but how much percentage he covers. In such cases it is necessary to be able to accurately estimate the percentage ratio which the issues related to the problem should be arranged for in terms of ascending complexity, and the starting point or the next step of the transition is determined from the applicant's technical level (junior, middle, senior, etc.).

Often encountered problem:  
Usually, a lower-level specialist is given a complicated question without answering it, the applicant's knowledge of the given problem may be estimated 0, whereas the applicant had some understanding and knowledge about the problem.  

To illustrate the organization of the correct sequence of technical questions, we should divide questions into two groups:

  1. Questions related to the concrete topic and classification of these questions by complexity.  
    
      Example (as an example setTimeout from WebAPIs will be considered).  
      Possible questions related to setTimeout in the correct order. 

      | | |
      | --- | --- |
      | 1 | - Describe setTimeout as a function.<br/>* Not important questions: <br/>1. Can the first argument of setTimeout not be a function? <br/>2. Is there a third argument for setTimeout, if yes, what does it represent and does it have limitations? If yes, then what kind of limitations? |
      | 2 | - Give a mathematical claim for the second argument of setTimeout. |
      | 3 | - Detailed description of setTimeout work. |
      | 4 | - Recursive setTimeout and setInterval. |
      | 5 | - setTimeout (fn, 0) as an exception. |
      | 6 | - Dom minimum timeout value. |
      | 7 | - setImmediate, setImmediate polyfill, polyfill implementation.<br /> * postMessage <br /> * messageChannel <br /> * <script> onreadystatechange |
      | 8 | - process.nextTick, Promise.resolve(). Compare with setTimeout() |
      | 9 | - Task, MicroTask, differences, execution order, implementation in different browsers. |
      | 10 | - setTimeouts’ execution order - FIFO, LIFO, random |

      Let's consider we do not set the correct sequence and start talking about setTimeout from Question 6 or its specific case, for example:  
       &#45; Please enter DOM_MIN_TIMEOUT_VALUE or DOM_CLAMP_TIMEOUT_NESTING_LEVEL in Google Chrome and FireFox.  
      In that case the wrong answer to the question or the lack of the response can not give information about the applicant's setTimeout knowledge.  

      **Use the right sequence of questions.**
  
  2. Topics that you can address only if the applicant is in line with that level.  
  
      Example - Questions related to engine.  
      
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
      
      Questions related to Web Assemble.
     
      * toolchain
        * emscripten
        * clang
        * llvm
      * Detailed description of webassembly work.
      * etc.
      
#### Common questions

The main questions are given separately (before or after) from the questions of the considered position, can also be held as a separate stage. The common questions, in their turn, are divided into two groups.

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

    **Note:** * This questionnaire can be changed depending on company requirements, considered position and the technical level of the applicant.
    
2. Questions related to the applicant's IT preferences

    | | |
    | --- | --- |
    | 1 | - Preferred Operating system |
    | 2 | - Preferred text editor or IDE |
    | 3 | - In addition to your basic programming language mention other languages you are interested in or want to work on. |
    | 4 | - How do you follow news? What resources do you use? |
    | 5 | - What goals does your GitHub account serve for (if you have any)? |  
    
    **Note:** Any question of this questionnaire as a separate question may not provide sufficient information about the applicant. However, the answer to all questions, as a whole, may allow you to understand the applicant’s world outlook in IT. For example: let’s review the answers of two different applicants.  
    
    Option 1.  
    
    | | |
    | --- | --- |
    | 1 | - Windows |
    | 2 | - Microsoft Visual Studio, WebStorm, Notepad++ |
    | 3 | - C#, Visual Basic, PHP |
    | 4 | - Looking for what I need in Google. I read Toster.ru and, in general, watch screencasts on Youtube.com |

    Option 2.  
    
    | | |
    | --- | --- |
    | 1 | - Linux, Unix-like operating systems. |
    | 2 | - Vim, Sublime Text or other text editor, but not IDE |
    | 3 | - C/C++, Rust, OCaml, Elixir (Erlang/OPT), Python |
    | 4 | - Medium, Hackernoon, Habr, Twitter... I am subscribed in Google and Mozilla Youtube channels |

    Note ... * Examples are from real life.  
    
#### The "last" question

**- Please rate your technical knowledge from 0 to 10.**

During the interview the tech. specialist will form an assessment that will be considered an alleged objective assessment and it is also important to get an assessment by the applicant. Additional assumptions may be made from the comparison of the two estimations.

### Task

The technical task presents technical issue representation corresponding to the considered position. The purpose of this method is to estimate the applicant's technical knowledge from the point of view of the implementation of practical tasks.  
The view points can be:

* Code quality
* Coding style
* Code architecture
* Naming convention
* File/Folder structure
* ...

##### Important points

* The estimation of the problem should be left to the applicant's discretion. The assessment of the complexity of his problem and the time/quality ratio may serve as additional information.
* The complexity of the task is not the main goal, and is mainly lower than the applicant's technical level.
* Task responses are desirable to be checked by several technical experts for more objective assessment.
* The task must have functional and technical specification and requirements.

### Quiz

Quiz or test work is a sequence of questions with possible answers. This method can be used for filtration of the preceding stages or as additional information in the main stages.

### Comparison

* Quiz
 * Advantage  
   Minor effort.
 * Disadvantage  
   Answering frequently asked questions and lack of oral conversation may be not an objective assessment.
* Task
 * Advantage  
   Opportunity to estimate practical work.
 * Disadvantage  
   Usually, "technical task" is done remotely, and lack of control and the availability of extra assistance affects the validity of the work estimation.
* Oral
 * Advantage  
   An objective assessment of theoretical knowledge, existence of oral conversation.
 * Disadvantage  
   In some cases, it is difficult to estimate the applicant's knowledge from his/her oral speech or self-reported problems.

- - - -

The Importance of Technical Interview
========

Any technical interviewing course unequivocally shows the technical level of the company.  
<br />
Based on the assessment of the tech. specialist, the company may employ the applicant. An incorrect assessment of the tech. specialist may cause problems later on.

- - - -

Disclaimer
========

The document does not aim to compile an ordered process of technical interview or interviewing stages for specific programming language, technology or company. The above mentioned points are the main clauses for technical interviews in IT. JavaScript is just an example. (For more detailed JavaScript questionnaire please refer the following [file](https://github.com/SurenAt93/Technical-Interview/blob/master/javascript.md) as an interview guide). The author tried not to define the stages of technical interview for keeping the document flexibility. The number and sequence of interview stages may vary depending on the programming language, the technology, the applicant's technical level, the company requirements and resources. The above mentioned points will be considered accurate also for the interviews related to specific libraries or frameworks. For example:  

JavaScript - ReactJs / NodeJs and etc.  
Python - Django and etc.  
Rust - Exonum and etc.  
...


- - - -

Notes
========

###### Note 1

The presence  of more than two tech․ specialists in the room (in which the interview will be conducted) can create an overwhelming atmosphere. The presence of a second tech. specialist is desirable for making more objective opinion. However, if tech. specialist is experienced and can conduct the interview alone, then the presence of one tech. specialist will be more optimal.

###### Note 2

At the end of the interview, regardless of the applicant's assessment or his / her potential mentor, give 5 minutes for the consultation, note mark the mistakes, give advice, guide and show the gaps in the technical knowledge. Send relevant links to articles, books or other resources to fill in the gaps. (Make the world a little bit better :slightly_smiling_face:)

Thank you.
- - - -
