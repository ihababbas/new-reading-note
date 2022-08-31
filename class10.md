# Class 10

## Understanding the JavaScript Call Stack

### What is a 'call'?
The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.
### How many 'calls' can happen at once?
 single call
### What does LIFO mean?
last in first out
### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
![alt text](stack.png)
### What causes a Stack Overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error
---
## JavaScript error messages

### What is a 'reference error'?
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
### What is a 'syntax error'?
this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
### What is a 'range error'?
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
### What is a 'type error'?
like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
### What is a breakpoint?
can  be achieved by putting a debugger statement in your code in the line you want to break.
### What does the word 'debugger' do in your code?
achieved the breakpoint

## Things I want to know more about

