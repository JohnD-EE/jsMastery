# jsMastery
Examples and  notes on JS


-----

**The groundwork for a new project**

-----

[About this project](about.md)

##Best Practices and Conventions
* Naming Conventions: Variables, Functions, Objects
* Variable Declarations (Use one var per scope)
* Decouple CSS, HTML etc.
* Decouple Event Handlers from Logic
* Respect Object Ownership
* Avoid Globals (Use Namespacing)
* Avoid Null Comparison
* Use Constants (e.g. a constants object for repeated values, UI Strings (e.g. messages to the user), URLS (e.g. BASE_URL), any value which might change (e.g. should be config)
* Performance (Avoid global lookups - going up the scope chain, avoid the with statement (creates its own scope and increases the scope chain,))


See https://github.com/rwaldron/idiomatic.js

##Foundations
* [Operators](operators.md) | [Operators Examples](qOperators.md)



##Javascript Types and Grammar

* [Types](types.md)
* [Type Coercion](types.md)
* etc
* 7 Built-in Types: null; undefined; boolean; number; string; object; symbol
* Variables don't have types but their values do
* Undefined vs Undeclared
* typeOf undefined  -  don't confuse with ReferenceError: not defined
* [Values](values.md)
* Values associated with types (null, numbers, strings etc.)
* [Native Objects](nativeObjects.md)
* type `this` into console for full list of standard built-in window objects
* 




##Javascript Functions, Scope and Context

* etc
* etc
* etc

##Lexical Environment and Scope Chain (finding variable values), Execution Context (this)

* etc


##Javascript Objects, Scope and Context

* etc
* etc
* etc

##Javascript Arrays

* etc
* etc
* etc


Asynchronous Callbacks

Event Queue and Execution Stack
When the execution stack is empty the Js engine looks at the event queue...