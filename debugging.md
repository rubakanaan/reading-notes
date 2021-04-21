# ERROR HANDLING AND DEBUGGING

*To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run*

### EXECUTION CONTEXT
JavaScript
Every statement in a script lives in one of three
execution contexts:
1. GLOBAL CONTEXT
    * Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT:
    * Code that is being run within a function.Each function has its own function context.
3. EVAL CONTEXT (NOT SHOWN): 
    * Text is executed like code in an internal function called eva l {) (which is not covered in this book). 

![exec](https://i.stack.imgur.com/eA9kM.png)


# UNDERSTANDING ERRORS 

*If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code.*

![handle](https://www.onlinetutorialspoint.com/wp-content/uploads/2015/04/Exception-Flow.png)


# HANDLING EXCEPTIONS

![trycatch](https://i.ytimg.com/vi/GYWUr7xlK-w/maxresdefault.jpg)

1. TRY:
    * First, you specify the code that you think might throw an exception within the try block. If an exception occurs in this section of code, control is automatically passed to the corresponding catch block.the try clause must be used in this type of error handling code, and it should always have eithera catch, fi na 1 ly, or both. If you use a continue, break, or return keyword inside a try, it will go to the f i na 11 y option.
2. CATCH:
    * If the try code block throws an
    exception, catch steps in with an
    alternative set of code.
    It has one parameter: the error
    object. Although it is optional,
    you are not handling the error if
    you do not catch an error.
    The ability to catch an error can
    be very helpful if there is an issue
    on a live website.
    It lets you tell users that
    something has gone wrong
    (rather than not informing them
    why the site stopped working). 
3. FINALLY:
    * The contents of the fi na 11 y
    code block will run either
    way - whether the try block
    succeeded or failed.
    It even runs if a return keyword
    is used in the try or catch block.
    It is sometimes used to clean up
    after the previous two clauses.
    These methods are similar
    to the .done(), . fail(), and
    . a 1 ways() methods in jQuery.
    You can nest checks inside each
    other (place another t ry inside a
    catch), but be aware that it can
    affect performance of a script. 