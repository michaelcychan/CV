# Coding Process Review
Date: 22 September 2022    

## Scorecard

*Exercise*: School results  
*Language*: JavaScript  

[Video](https://youtu.be/5qnM59Da3_0)  

## I use an agile process
Rating: **Strong**  
You began your information gathering by first clarifying the inputs and outputs of the system, which was a great first step to take. Following this, you clarified on edge cases with the user, which was a great place to go, and resulted in you getting a very solid overall idea of the system.  

You have also used your input-output table to record the behaviours for the core functionality and some of the edge cases.  

You have done comprehensive information gathering concerning edge cases.  

## I can model anything
Rating: *Steady*  
You were able to discern that this problem required state due to having to be able to call the addScores() method multiple times and keeping those test scores over the object's lifespan. This led you to the utilisation of a class with a constructor that created this state variable.  

I suggest that you ensure that you follow Javascript conventions for your method names i.e. camelCase.  

You were on the right path with your algorithm, but due to the time constraint, you were making some good progress with the algorithm.  

## I can TDD anything
Rating: *Steady*   
You were doing end-to-end testing based on the behaviours of the program which was a great way to encode the requirements of the program into the algorithm. This also increases the flexibility that you have in changing/refactoring the code.  

Just be careful of testing for incorrect outputs and ensure that you have the outputs in your test aligned with the acceptance criteria. I had to warn you that the 0 counts needed to be included in the output when you were doing your simplest input strings.  

You were loosely following the RGR cycle and did refactor on some of the refactor phases, but there were some refactor phases that were skipped.  

## I can program fluently
Rating: **Strong**  
You seemed comfortable enough using the terminal and editor to set up your environment.  

You seemed to have a sufficient level of knowledge in all of the relevant programming constructs needed to solve the problem.  


## I can refactor anything
Rating: Improving  
You were aware of refactoring your code, but when the opportunity came to extract a method, you did not do so. Once a method has more than one responsibility, that is a good time to extract logic to a new method so that the code adheres to the single-responsibility principle.  

## I can debug anything
Rating: **Strong**  
You regularly read the stack trace to ensure that you are up-to-date on all possible bugs. You have also used documentation effectively to understand which methods would be useful to solve the problem and what the syntax would be.  

## I write code that is easy to change
Rating: *Steady*  
I was pleased to see that you had your test suite decoupled from the implementation. This was done by testing the expected inputs and outputs of the system. This promotes flexibility in your code, and so any changes made to the structure of the code will not warrant a change in tests.  

Your variable and method names were very descriptive and aided in code readability which in turn helps to make code easier to change.  

You have committed whenever your tests pass which aids in being able to roll back to a previous safe version if you were to run into any trouble with new additions to the code or refactors. I would just suggest that you make the commit messages more descriptive of what features were covered and what specifically was refactored so that there is a more clear commit history that anybody can reference and understand.  

## I have a methodological approach to problem solving
Rating: *Steady*  
You mostly adhere quite closely to the RGR cycle. There is one refinement that I would suggest and that is to try to identify code that can be refactored into separate methods before moving from a refactor phase to the next red phase. Method extractions help to build the overall design of the algorithm and create clean code in an incremental manner. This leads to less risk of bugs creeping in when complicated refactoring is done later in the development process because it was left to be done later on.  

You have aimed to provide the client with immediate value by prioritising the core cases over the edge cases except for when you tested for the generateReport() method when no scores were added.  

## I can justify the way I work
Rating: *Steady*  
You were vocal throughout the session, which helped me understand your thought process. However, you deviated from the process without any justification when you were skipping refactor phases. I recommend that you provide sound justifications grounded in the process you’ve learnt at Makers for an effective development workflow.  

## General feedback
This was a great 5th review session. The one main thing that you could focus on is identifying how the code can be refactored on the refactor phases.