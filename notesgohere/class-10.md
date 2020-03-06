## Execute order 66

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasking cannot complete until another statement or function has been run.   

### The stack, it resolves
When a statement has to call some other code in order to do it's job, the new task goes to the top of the pile of things to do. Once the enw task has been performed, the interpreter can go back to the task in hand. Each time a new item is added to the stack, it creates a new execution context. Variables defined in a function are only available in that function. If that function gets called a second time, the variables can have different values.   

Each time a script enters a new execution context, there are two phases of activity.  
 - Prepare
    - New scope is created.
    - Variables, functions, and arguments are created
    - the value of this keyword is determined
 - Execute
    - Now it can assign values to variables
    - Reference functions and run their code
    - Execute statements

_hoisting_ Calls functions before they have been delcared, and assigns a value to a variable that has not yet been declared.
#### Error object
_Error_ Generic error, the other errors are based on this one  
_Syntax Error_ Syntax has not been followed  
_ReferenceError_ Tried to reference a vairiable that is not delcared/within scope  
_TypeError_ An unepected data type that cannot be coerced  
_RangeError_ Numbers not in acceptable range  
_URIError_ encodeURI(), decodeURI(), and similar methods used incorrectly  
_EvalError_ eval() function used incorrectly  

#### debugging workflow 
First, where is the problem? Now, what exactly is the problem?  
You can use breakpoints to pause the execution of the script and see what value the variables are returning. If there are multiple variables, you can step through them one-by-one.  
Conditional breakpoints are variables that you can access only if a condition has been met (i < 20; i = 19)  