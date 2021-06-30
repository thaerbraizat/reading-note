# FUNCTIONAL PROGRAMMING
 ![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1.What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

2. What is a pure function and how do we know if something is a pure function?

A pure function is a function which: Given the same input, will always return the same output. Produces no side effects.

3. What are the benefits of a pure function?

Pure functions are much easier to read and reason about. All relevant inputs and dependencies are provided as parameters, so no effects are observed that alter variables outside of the set of inputs. This means that we can quickly understand a function and its dependencies, just by reading the function's declaration.

4. What is immutability?

In JavaScript, only objects and arrays are mutable, not primitive values. (You can make a variable name point to a new value, but the previous value is still held in memory. ... Immutables are the objects whose state cannot be changed once the object is created. Strings and Numbers are Immutable.

5. What is Referential transparency?

A function is referentially transparent if it's a pure function whose parameters are immutable. ... To achieve this in JavaScript we use immutable-js to create immutable data, and closures to make sure observers can't introspect our object and mutate its state.

## Node JS Tutorial for Beginners #6 - Modules and require()

1. What is a module?

Module pattern. The Module pattern is used to mimic the concept of classes (since JavaScript doesn't natively support classes) so that we can store both public and private methods and variables inside a single object — similar to how classes are used in other programming languages like Java or Python.

2. What does the word ‘require’ do?

require function is the easiest way to include modules that exist in separate files

3. How do we bring another module into the file the we are working in?

Modules are created in Node.js by creating a JavaScript file. Every time you create a new file with .js extension, it becomes a module.we have to export the functions and import them in the file we want to call the functions.

4. What do we have to do to make a module available?

we set a module inside the variable and then export then you call the variable and use the module.






## Things I want to know more about


### Resource
* [Functional Programming Concepts](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design).
* [Node JS Tutorial for Beginners #6 - Modules and require()](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design).
