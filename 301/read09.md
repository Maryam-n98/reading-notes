# Read 09: Readings: FUNCTIONAL PROGRAMMING


### What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### What is a pure function and how do we know if something is a pure function?
The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?
So how do we know if a function is pure or not? Here is a very strict definition of purity:
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects.

### What are the benefits of a pure function?
Pure functions benefits
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D
A simple example would be a function to receive a collection of numbers and expect it to increment each element of this collection.

### What is immutability?
 immutability is important to make our functions more consistent and predictable. The idea is to build a new collection with all absolute values.

 ### What is Referential transparency?
 In maths, referential transparency is the property of expressions that can be replaced by other expressions having the same value without changing the result in any way.



### What is a module?
 Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

 ### What does the word ‘require’ do?
 The require() function will return an object, function, property or any other JavaScript type, depending on what the specified module returns.

 ### How do we bring another module into the file the we are working in?

 module.exports = { add }

 ### What do we have to do to make a module available?
we have added the add() function to module.exports object. Adding the function to module.exports will make it available in any file that imports the js file module.


