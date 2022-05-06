TURING MACHINE (TM) LAMBDA CALCULUS CONVERTER
========================

[This is web application that hosts two interpreters: the lambda calculus interpreter and Turing machine interpreter, and allows the user to simulate between them using the methods outlined by Dal Lago and Martini.](https://nunoagoncalves.github.io/Lambda-Calculus-Interpreter/)

The web application works in both directions outlined by Dal Lago and Martini. The application can simulate from the lambda calculus to the multi-tape Turing machine, as well as from the single-tape Turing machine to the weak lambda calculus.

- Built in the **HTML/CSS/JavaScripts**
- User Interface built with **Bootstrap**, **JQuery**, and **FullPages**
- Tested using **Jest** and **Node.JS**

The lambda calculus interpreter uses an applicative-order evaluation strategy to perform beta reduction. The interpreter can reduce complicated lambda expressions, highlight the parameter and argument of a reduction, and simulate SKI combinators and boolean logic.

The TM interpter works using a JSON-based terminal as outlined by Chad Palmer in his article 'A Complete Web Page: Building a Turing Machine in JavaScript'. The TM interperter can visualise the run of the TM by simulating the machine head on the tape.

The multi-tape TM interpreter is used for simulating the lambda calculus term in a Turing machine. 

INSTRUCTIONS FOR SIMULATING TURING MACHINE (TM) IN THE LAMBDA CALCULUS
================================

1. In the `Single-Tape Turing Machine Interpreter`, run a TM using either an example in the drop-down list or create a TM of your own

2. In the `Lambda Calculus Interpreter`, enter 'T' to denote the beginning of the TM as a lambda term

3. In the `Lambda Calculus Interpreter`, enter to the right of 'T' the tape you want to run:

        T101

4. Run the `Lambda Calculus Interpreter`

INSTRUCTIONS FOR SIMULATING LAMBDA CALCULUS IN THE MULTI-TAPE TURING MACHINE (TM)
================================

1. In the `Lambda Calculus Interpreter`, enter the lambda calculus term being converted.

2. In the `Multi-Tape Turing Machine Interpreter`, the lambda calculus term previously entered should now be converted into its Dal Lago and Martini notation

3. Run the `Multi-Tape Turing Machine Interpreter`

4. The tape of the interpreter at the halting state will be the weak beta normal form of the lambda calculus term in Dal Lago and Martini notation

LAMBDA CALCULUS INTERPRETER
========================

![](img/lambdaGif.gif)
 
TURING MACHINE (TM) INTERPRETER
========================

<img src="img/turingGif.gif" width="750" height="450">

MULTI-TAPE TURING MACHINE (TM) INTERPRETER
========================

<img src="img/multitapeGif.gif" width="800" height="500">

FILES
===============

- `lambda_calculus_interpreter.js`: The lambda calculus system and the interpreter for running and reducing the lambda calculus terms
- `single_tape_TM_interpreter.js`: The TM and its interpreter for running the TM
- `multi_tape_TM_interpreter.js`: The multi-tape interpreter used to simulatie the lambda calculus in the multi-tape TM interpreter
- `simulation_TM_to_lambda_calculus.js`: The functions necessary to convert the single-tape TM into a lambda calculus term 

DEPENDENCIES & REFERENCES
===================

Thanks go to the following authors/resources for their help

[jQuery](https://jquery.com/)  
[jQuery Terminal](https://terminal.jcubic.pl/)  
[BootStrap](https://getbootstrap.com/)  
[fullPage.js](https://alvarotrigo.com/fullPage/)  
[Chad Palmer](https://medium.com/swlh/a-complete-web-page-building-a-turing-machine-in-javascript-d6c32d3708c4)  
[Tadeu Zagallo](https://tadeuzagallo.com/blog/writing-a-lambda-calculus-interpreter-in-javascript/)  



