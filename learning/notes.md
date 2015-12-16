# Notes from dev talks and tutorials


## Eric Elliott -  Fluent 2014 JavaScript Talk - Static Types are Overrated 

- type correctness does not guarantee program correctness!
- you should be using automated testing for every program
- use *jshint* - variable name typos, underfined variables, unused variables, cyclomatic complexity
- *tern.js* - autocompletion on variables and properties, function argument hints...
- *trace.gl* - for debugging - records every single function call, traces every value as it flows through program
- *dominators view* in chrome dev tools - making sure objects are being garbage collected
- automated testing - keep your modules small and independent
- write tests first
- jsdoc static analysis - tern can parse jsdoc for type hints - DocBlockr SublimeText
- you can use .map() on strings

## Eric Elliot - The Two Pillars of JavaScript: How to Escape the 7th Circle of Hell

- Once Upon a Time. I was trapped in the darkness. I was blind.
- JavaScript offers something other languages lack: **Freedom!**
- JavaScript popularized two paradigms which are extremely important for the evolution of programming:
	-- Prototypal Inheritance (objects without classes, and prototype delegation, aka OLOO — Objects Linking to Other Objects), and
	-- Functional Programming (enabled by lambdas with closure)
- I like to call these paradigms the two pillars of JavaScript
- JavaScript is pretty good at letting you code poorly if you don’t bother to learn it properly
- If you’re creating constructor functions and inheriting from them, you haven’t learned JavaScript
- “Those who are not aware they are walking in darkness will never seek the light.” ~ Bruce Lee
- Constructors violate the open/closed principle because they couple all callers to the details of how your object gets instantiated.
- In JavaScript, factory functions are simply constructor functions minus the `new` requirement, global pollution danger and awkward limitations (including that annoying initial capitalized letter convention).
- JavaScript doesn’t need constructor functions because any function can return a new object.
- “The problem with object-oriented languages is they’ve got all this implicit environment that they carry around with them. You wanted a banana but what you got was a gorilla holding the banana and the entire jungle.” ~ Joe Armstrong
- Problems: The Gorilla / Banana problem, The Tight Coupling Problem, The Duplication by Necessity Problem
- The `class` keyword will probably be the most harmful feature in JavaScript.
- Other good alternatives include making better use of JavaScript modules as an alternative to inheritance (I recommend npm and ES6 modules with Browserify or WebPack), or simply cloning objects by copying properties from a source object to a new object (e.g. `Object.assign()`, `$.extend()`, `_.extend()`, etc…).
