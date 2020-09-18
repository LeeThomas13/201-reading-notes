# Refactoring
<br>

[Link to Article 1](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
<br>

“Complexity is anything that makes software hard to understand or to modify."
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data So how do we know if a function is pure or not? Here is a very strict definition of purity:
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

Functions as first-class entities can:
refer to it from constants and variables
pass it as a parameter to other functions
return it as result from other functions

Higher-order functions
When we talk about higher-order functions, we mean a function that either:
takes one or more functions as arguments, or
returns a function as its result
The doubleOperator function we implemented above is a higher-order function because it takes an operator function as an argument and uses it.
You’ve probably already heard about filter, map, and reduce. Let's take a look at these.
Filter Map Reduce

[Link to Article 2](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)
<br>

Refactor into one line when applicable 
function showProfile(user) {
  if (user.authenticated === true) {
    // ..
  }
}

// Refactor into ->

function showProfile(user) {
  // People often inline such checks
  if (user.authenticated === false) { return; }

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)