# Notes from dev talks and tutorials


## Eric Elliott -  Fluent 2014 JavaScript Talk - Static Types are Overrated 

- type correctness does not guarantee program correctness!
- you should be using automated testing for every program
- Use *jshint* - variable name typos, underfined variables, unused variables, cyclomatic complexity
- *tern.js* - autocompletion on variables and properties, function argument hints...
- *trace.gl* - for debugging - records every single function call, traces every value as it flows through program
- *dominators view* in chrome dev tools - making sure objects are being garbage collected
- automated testing - keep your modules small and independent
- write tests first
- jsdoc static analysis - tern can parse jsdoc for type hints - DocBlockr SublimeText
- you can use .map() on strings

