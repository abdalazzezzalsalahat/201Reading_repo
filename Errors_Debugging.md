# Errors
> **If a JavaScript statement generates an error, then it throws an exception.**
> **At that point, the interpreter stops and looks for exception-handl ing code.**
## ORDER OF EXECUTION 
> ***The JavaScript interpreter uses the concept of execution contexts.***
**There is one global execution context; plus, each function creates a new new execution context.**
> *They correspond to variable scope.*
1. PREPARE
    - *The new scope is created*
    - *Variables, functions, and arguments are created*
    - *The value of the this keyword is determined*
2. EXECUTE
    - **Now it can assign values to variables**
    - **Reference functions and run their code**
    - **Execute statements**


### ERROR OBJECTS
`Error`, `SyntaxError`, `ReferenceError`, `TypeError`, `RangeError`, `URIError`, `EvalError` ,`name` ,`message`, `fileNumber`, `lineNumber `

### ERROR TYPES
*- Syntax Error: Incorrect syntax*
*- Reference Error: variable doesn't exist*
*- URI Error: Incorrect use of URI function*
*- Eval Error: Incorrect use of eval() function*
*- Type Error: value is unexpected data type*
*- Range Error: number outside of range*
*- Error: genaric error object*
*- NaN: not a number*



# debugging

## DEBUG THE SCRIPT TO FIX ERRORS
> **Debugging is about deduction: eliminating potential causes of an error.**
> **Here is a workflow for techniques you will meet over the next 20 pages.**
> **Try to narrow down where the problem might be, then look for clues.**

*`WHERE IS THE PROBLEM?`*
*`WHAT EXACTLY IS THE PROBLEM?`*

1. `console.info('And we\'re off ... ' );`
2. `console.table(contacts);`
3. ```$('form input[type="text"]').on('blur',function() {
        console.assert(this.value > 10, 'User entered less than 10');
    });```
### DEBUGGER KEYWORD
> **creating a breakpoint in the code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.**
> **`debugger;`**
## HANDLE ERRORS GRACEFULLY
- **TRY**
> **First, you specify the code that you think might throw an exception within the try block.**

- **CATCH**
> **If the try code block throws an exception, catch steps in with an alternative set of code.**

- **FINALLY**
> **The contents of the fina11y code block will run either way, *whether the try block succeeded or failed.***
```
response= ' {"deals" : [{"title" : "Farrow and Ball", . . . '}]};
if (response) {
    try{
        var dealOata = JSON . parse(response);
        showContent (dealData);
    }
    catch(e) {
        var errorMessage = e.name + ' ' + e .message;
        console.log(errorMessage);
        feed.innerHTML = '<em>Sorry, could not load deals</em>';
    }
    finally {   
        var link= document.createElement('a');
        link.innerHTML = '<a href="tr y-catch-fi nally.html">rel oad<la>';
        feed.appendChild{link);
    }
}
```
> **If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.**
> **Use them to give your users helpful feedback.**