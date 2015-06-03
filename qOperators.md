#Operators Examples


```js
var a = 1 + 2 * 10;
console.log(a); //21
```
Returns 21, not 30 as might be expected. The multiplication operator has a higher precedence than the addition operator so (2 * 10) will be evaluated first. 
**Concepts: Operator Precedence**

```js
var a = 3,
    b = 4,
    c = 5;
console.log (a = b = c); //5
console.log (b); //5 
```
Returns 3, the assignment operator ('=') uses right-to-left associativity so firstly b is assigned the value of c which is 5, and then a is assigned the new value of b.
**Concepts: Associativity**




