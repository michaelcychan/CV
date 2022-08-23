# Coding Process Review
Start date: Mon 11 July 12:00pm BST  
End date:   Mon 11 July 1:00pm BST  

Recording: https://youtu.be/GSrpFcar2oQ  

## Scorecard
Exercise: Band pass filter  
No show?: No  
Language: JavaScript  

**I use an agile process**  
*Rating: Steady*  
You did a pretty good job gathering the main requirement from the client and asked a lot of pertinent questions. You were able to identify a lot of finer details such as that the frequencies will always be integers and the fact that the upper and lower limit should have default values of 1000 and 40 respectively. You also identified edge cases: no numbers present in the input array and corrupted input.  

Your input-output table is still very brief and contains only 1 example of an input-output pair. It is often helpful to have a list of examples to guide your development process and to serve as a reference. You can always extrapolate additional input-output cases from the examples the client gives you or simply request more examples from the client.  

**I can model anything**  
*Rating: Strong*  
You chose to use the function to solve this problem which is the appropriate abstraction given that the problem is stateless.
You adhered to naming best practices for your parameters, variables and function. You used camelCase for your function name(‘BandPassFilter’) and for your variables and parameters. While your variables and parameters were descriptive and contextual, it is best practice to name your function using a verb and not a noun for example ‘filter’ or ‘filterSoundwave’ or ‘applyFilter’  
Your algorithm makes sense as it iterates through the input array and transforms each element according to the upper and lower limit.  

**I can TDD anything**  
*Rating: Improving*    
You started with a simple test case: interrogating the behaviour of your filter when given an array of frequencies that are within the specified range. Your second test was also similar to your first one. Yes, the tests were simple but they could have been simpler. It would have been simpler to have your test case input be an array with just one value that is within range. Then your subsequent tests can still have one input frequency but on either side of the range.  

In addition, the simplest way to make a test pass is to return a hardcoded value that satisfies the test condition. Hardcoded values also have the benefit of allowing for patterns in the solution to develop which can be leveraged in the refactor phase.  

**I can program fluently**  
*Rating: Steady*  
You were fluent in your use of the command line. You were also familiar with language construct and showed that you understand array manipulation by using the built-in map method to iterate and transform your array.  

Your algorithm was also logical and solved the problem in one of the most efficient ways (iterating and checking each element of the array using a built-in method).  

**I can refactor anything**
*Rating: Improving*  
I did not get to see any significant use of the refactor phase to either remove hardcoded values and generalize or two extract functions from your main function out of sections of code in your main function that are complex enough to stand alone. Remember generalizing in the green phase will not only necessitate the introduction of complexity but also means that refactoring in the refactor phase of the RGR cycle becomes significantly harder. In addition, it is not the simplest way to make a test pass.

**I can debug anything**  
*Rating: Steady*  
You are familiar with common errors and interpret most of what you see in the command line and stack trace well. You also form a hypothesis about the error you are seeing and then act on said hypothesis instead of making random changes to your code to try to resolve errors. I also like the fact that you printed to the console to try to get a better understanding of what was happening in your function. You also looked up documentation on the syntax for throwing and catching errors.  

**I write code that is easy to change**  
*Rating: Improving*  
I, unfortunately, did not get to see you make use of git. It is good practice to do a commit each time you either enter the green phase or refactor. This way, it is much easier to roll back any breaking changes that you introduce. Your commit message also has to be descriptive.  

Your code was decoupled from your test suite because it had the behaviour-first approach. What this means is that since you’re not testing for implementation details, any changes in how you implement your algorithm will not result in your test suite having to change.  

**I have a methodological approach to problem solving**
*Rating: Steady*
You followed a regular RGR cycle and showed that you understand the underlying principle behind the RGR cycle. You also prioritized core cases and only addressed edge cases after having a working solution for core cases.  

Your tests also progressed in a logical order: you started with a situation wherein the soundwave does not need transformation and then proceeded to situations where transformation is needed on only one aspect(either below or above range).  

You looked up documentation on how to throw errors and how to subsequently catch them in your tests.  

**I can justify the way I work**  
*Rating: Strong*  

You vocalized your process very well and it was clear what you were doing. You also reasoned well and justified all the decisions you made regarding your algorithm. Even when stuck, you still justified and reasoned every attempt that you made at a solution to the non-compliant test.  

## General feedback
Well done on having a working solution and although you got stuck in the end when dealing with an edge case, you still had a working solution and showed a calculated and methodical approach to debugging. Remember that the best tests are the simplest ones and equally, the simplest way to make a test pass is to return a hardcoded value. That way, you get to see the value that the refactor phase of the RGR cycle brings with it.  

You also did very well in the information gathering phase by asking good questions and identifying both edge cases and the finer details of the problem. This is a notable improvement from your last exercise!  

You have a pretty solid understanding of TDD and I think you’ll do better in your next exercise.
