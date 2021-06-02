## JavaScript book, Ch. 10, “Error Handling & Debugging”

The JavaScript interpreter uses the concept of **execution contexts.** 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope.


* If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code. 
If you are anticipating that something in your code 
may cause an error, you can use a set of statements 
to handle the error 
This is important because if the error is not handled, 
the script will just stop processing and the user will 
not know why. So exception-handling code should 
inform users when there is a problem.


* Whenever the interpreter comes across an error, 
it will look for error-handling code. In the diagram 
below, the code has the same structure as the code 
you saw in the diagrams at the start of the chapter. 
The statement at step 1 uses the function in step 2, 
which in turn uses the function in step 3. Imagine 
that there has been an error at step 3. 

When an exception is thrown, the interpreter 
stops and checks the current execution context for 
exception-handling code. So if the error occurs in the 
getName () function (3), the interpreter starts to look 
for error handling code in that function. 


* If an error happens in a function and the function 
does not have an exception handler, the interpreter 
goes to the line of code that called the function. 
In this case, the get Name () function was called by 
greetUser(), so the interpreter looks for exceptionhandling code in the greetUser() function (2). 
If none is found, it continues to the next level, 
checking to see if there is code to handle the error 
in that execution context. It can continue until it 
reaches the global context, where it would have to it 
terminate the script, and create an Error object. 


* So it is going through the stack looking for errorhandling code until it gets to the global context. 
If there is still no error handler, the script stops 
running and the Error object is created.




## HOW TO DEAL WITH ERRORS



*  DEBUG THE SCRIPT TO FIX ERRORS 
If you come across an error while writing a script 
(or when someone reports a bug), you will need to 
debug the code, track down the source of the error, 
and fix it. 

You will find that the developer tools available in 
every major modern browser will help you with 
this task. In this chapter, you will learn about the 
developer tools in Chrome and Firefox. (The tools in 
Chrome are identical to those in Opera.) 
IE and Safari also have their own tools (but there is 
not space to cover them all). 


* HANDLE ERRORS GRACEFULLY 
You can handle errors gracefully using try, catch, 
throw, and f i na 1 ly statements. 
Sometimes, an error may occur in the script for a 
reason beyond your control. For example, you might 
request data from a third party, and their server 
may not respond. In such cases, it is particularly 
important to write error-handling code. 



## WHERE IS THE PROBLEM? 


**First** should try to can narrow down the area where 
the problem seems to be. In a long script, this is 
especially important. 

1. Look at the error message, it tells you: 
• The relevant script that caused the problem. 
• The line number where it became a problem for 
the interpreter. (As you will see, the cause of 
the error may be earlier in a script; but this is the 
point at which the script could not continue.) 
• The type of error (although the underlying cause 
of the error may be different). 


2. Check how far the script is running. 
Use tools to write messages to the console to tell 
how far your script has executed. 


3. Use breakpoints where things are going wrong. 
They let you pause execution and inspect the values 
that are stored in variables. 


If you are stuck on an error, many programmers 
suggest that you try to describe the situation (talking 
out loud) to another programmer. Explain what 
should be happening and where the error appears 
to be happening. This seems to be an effective way 
of finding errors in all programming languages. (If 
nobody else is available, try describing it to yourself.) 


**WHAT EXACTLY IS THE PROBLEM?**

Once you think that you might know the rough area 
in which your problem is located, you can then try to 
find the actual line of code that is causing the error. 


1. When you have set breakpoints, you can see if the 
variables around them have the values you would 
expect them to. If not, look earlier in the script. 


2. Break down I break out parts of the code to test 
smaller pieces of the functionality. 
• Write values of variables into the console. 
• Calrfunctions from the console to check if they 
are returning what you would expect them to. 
• Check if objects exist and have the methods I 
properties that you think they do. 


3. Check the number of parameters for a function, or 
the number of items in an array. 
And be prepared to repeat the whole process if the 
above solved one error just to uncover another ... 
If the problem is hard to find, it is easy to lose track 
of what you have and have not tested. Therefore, 
when you start debugging, keep notes of what you 
have tested and what the result was. No matter 
how stressful the circumstances are, if you can, 
stay calm and methodical, the problem will feel less 
overwhelming and you will solve it faster. 


## summary

* If you understand execution contexts (which have two 
stages) and stacks, you are more likely to find the error 
in your code.


* Debugging is the process of finding errors. It involves a 
process of deduction. 


* The console helps narrow down the area in which the 
error is located, so you can try to find the exact error. 


* JavaScript has 7 different types of errors. Each creates 
its own error object, which can tell you its line number 
and gives a description of the error. 

* If you know that you may get an error, you can handle 
it gracefully using the try, catch, finally statements. 
Use them to give your users helpful feedback.