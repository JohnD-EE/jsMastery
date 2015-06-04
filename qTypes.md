#Types Examples

**Concept** Dynamic Typing (aka Loose Typing) 

```js
var a; 
a = 10;
a = {};
a = [];
a = true;
a = null;
a = "Hello";
console.log( typeof(a) ); // "string"
```
The js engine works out what type during execution. Some languages use static typing so once the type is declared it can't be changed.


**Concept** Numbers

```js
typeof(NaN); //"number"
```
NaN (Not a Number) is a number property

```js
typeof(Number("egg")); //"number"
Number("egg"); //NaN
Number.NaN; //NaN
```
The engine is asked to coerce "egg" into a number.  It does this but returns 'NaN' because "egg" can't be coerced to a numerical value. NaN is a property of the javascript "number" type.
Nan is a property of Number.

Number

Primitive type = something that isn't an object - a single value:
Undefined - doesn't exist...   

Null - has no value

Boolean:  true or false

number = floating point / doesn't have integer / decimal etc.

string = ""    ''

SYMBOL (ES6) 

##Type Coercion
