# functional programming

* Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

* pure functions :It returns the same result if given the same arguments,and It does not cause any observable side effects


* when my function will be impure  which is a function that uses a global object that was not passed as a parameter

1. Reading Files :If our function reads external files, it’s not a pure function
2. Random number generation



* Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen

* Basically, if a function consistently yields the same result for the same input, it is referentially transparent

> pure functions + immutable data = referential transparency

* Higher order functions are functions that take multiple arguments or return a function as its result

# Refactoring JavaScript to be more Readability

* Like giving spaces between every block of code to make it more tidy.

* write one function that accepts a list of friendly things

* separated some logic and reduced the number of lines of code

* Using understandable variable names

*  adding comments so we can know this for what or what doing 

