<a href = "https://n-alex-goncalves.github.io/Turing-Machine-Lambda-Calculus-Converter/">
<img src="img/logo.PNG">
</a>

This is a web application that provides an interpreter for interpreter and translating between the lambda calculus system and Turing machines. The application can translate in both directions, converting from the weak lambda calculus to the multi-tape Turing machine, or from the single-tape Turing machine to the weak lambda calculus. The methods used for these translations are based on those outlined by Dal Lago and Martini in their paper ["The Weak Lambda Calculus as a Reasonable Machine"](https://dl.acm.org/doi/10.1016/j.tcs.2008.01.044).

- Built in **HTML/CSS/JavaScript**
- User Interface built with **Bootstrap**, **JQuery**, **JQuery Terminal** and **FullPages**
- Tested using **Jest** and **Node.JS**

Website: https://n-alex-goncalves.github.io/Turing-Machine-Lambda-Calculus-Converter/

## GENERAL DESCRIPTION

The lambda calculus interpreter uses an applicative-order evaluation strategy to perform beta reduction. The interpreter is able to simplify complex lambda calculus expressions. It can also highlight the parameters and arguments of an expression, and it can simulate both SKI combinators and boolean logic operations.

The Turing machine (TM) interpter works using a JSON-based terminal as outlined by Chad Palmer in his article ["A Complete Web Page: Building a Turing Machine in JavaScript"](https://medium.com/swlh/a-complete-web-page-building-a-turing-machine-in-javascript-d6c32d3708c4). The TM interperter can visualise the run of a Turing machine by simulating the movement of the machine head on a tape.

The multi-tape TM interpreter is used for simulating a lambda calculus term in a Turing machine. The format of the lambda term that is simplified by the multi-tape interpreter is similar to the format of De Brujin indices.

## INSTRUCTIONS FOR SIMULATING TURING MACHINE (TM) IN THE LAMBDA CALCULUS

1. In the `Single-Tape Turing Machine Interpreter`, run a TM using either an example in the drop-down list or create a TM of your own

2. In the `Lambda Calculus Interpreter`, enter 'T' to denote the beginning of the TM as a lambda term

3. In the `Lambda Calculus Interpreter`, enter to the right of 'T' the tape you want to run:

        T101

4. Run the `Lambda Calculus Interpreter`

## INSTRUCTIONS FOR SIMULATING LAMBDA CALCULUS IN THE MULTI-TAPE TURING MACHINE (TM)

1. In the `Lambda Calculus Interpreter`, enter the lambda calculus term being converted.

2. In the `Multi-Tape Turing Machine Interpreter`, the lambda calculus term previously entered should now be converted into its Dal Lago and Martini notation

3. Run the `Multi-Tape Turing Machine Interpreter`

4. The tape of the interpreter at the halting state will be the weak head normal form of the lambda calculus term in Dal Lago and Martini notation

## INTERPRETER SHOWCASE

### LAMBDA CALCULUS INTERPRETER

![](img/lambdaGif.gif)
 
### TURING MACHINE (TM) INTERPRETER

<img src="img/turingGif.gif" width="740" height="450">

## FILES

- `lambda_calculus_interpreter.js`: The lambda calculus system and the interpreter for running and reducing the lambda calculus terms
- `single_tape_TM_interpreter.js`: The TM and its interpreter for running the TM
- `multi_tape_TM_interpreter.js`: The multi-tape interpreter used to simulatie the lambda calculus in the multi-tape TM interpreter
- `simulation_TM_to_lambda_calculus.js`: The functions necessary to convert the single-tape TM into a lambda calculus term 

## DEPENDENCIES & REFERENCES

Thanks go to the following authors/resources for their help and guidance:

[jQuery](https://jquery.com/)  
[jQuery Terminal](https://terminal.jcubic.pl/)  
[BootStrap](https://getbootstrap.com/)  
[fullPage.js](https://alvarotrigo.com/fullPage/)  
[Chad Palmer](https://medium.com/swlh/a-complete-web-page-building-a-turing-machine-in-javascript-d6c32d3708c4)  
[Tadeu Zagallo](https://tadeuzagallo.com/blog/writing-a-lambda-calculus-interpreter-in-javascript/)  
