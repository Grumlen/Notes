#Eloquent JavaScript 2nd Edition

##Introduction

Programming language exist so that we can instruct computer how to accomplish a given task, and essentially act as an interface between how we understand commands and the binary language that a computer understands.

##Chapter 1

A value is a reserved collection of bits that represents some piece of information. There are 6 types of values: numbers, strings, Booleans, objects, functions, and undefined. A number value is exactly that: a number. A string value is a sequence of characters, with a "\" preceding special characters. Boolean values are "true" or "false", often generated through an operator comparing other values.

Operators are actions that are performed on values, such as the arithmetic operators. Unary operators only accept one value, binary operators accept 2 values, and ternary will accept 3 values.

JavaScript will engage in automatic type conversion of values if you are not careful, so be aware of how it may be interpreting the values when used with various operators.

##Chapter 2

Variables provide a way of storing values for use later, and the name of the variable can be used in place of the value in all instances after it is declared. multiple variables can be declared at once by using a comma to separate them.

Functions are values that are generated by executing operations on passed values. They can also generate side-effects, such as displaying content. Examples include console.log(), alert(), prompt(), and confirm().

Conditional execution allows for you to create conditions for executing certain parts of a program. If/Else, While, Do/While, For, and Switch/Case are examples of how you can create code to run 0, 1, or multiple times if necessary. Generally conditional code should be wrapped in {} to separate it from the main content block. A "break" command can be included in a conditional to immediately break out of the block and go to the next line in the parent block. When using a switch structure you must include breaks to exit the block.

Comments are useful for denoting the purpose of sections of code so that you or others can easily edit the code later if necessary.

##Chapter 3

Functions can be defined either using "var NAME = function(VALUE) {}" (created function right there) or "function NAME(VALUE) {}" (creates function at beginning of program) with the code for the function going inside the brackets. A function can accept any number of parameters, including none. If not enough parameters are supplied when calling the function,  they default to undefined. If too many are supplied, the extra parameters are ignored. Functions also create a localized scope, meaning that any variables created through the "var" command only exist within the function, even if that variable exists globally outside the function.

Functions can be nested inside each other or made recursive (when a function calls upon itself in its own block). The stack is created as a result of nested functions, with every function being added to the top and the stack always being resolved top-down.

Creating new functions should occur when they have a clearly defined purpose and the code within them will need to be used multiple times within the program. Functions can have a side effect and/or return a value. A side effect is when a function performs some action other than returning a value that is useful, such as printing specific text. A pure function is one that has no side effects and relies ONLY on local variables, such that it always produces the same results when given the same parameters.