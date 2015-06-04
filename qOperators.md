#Operators Examples

**Concept:** Operator Precedence
```js
var a = 1 + 2 * 10;
console.log(a); //21
```
Returns 21, not 30 as might be expected. The multiplication operator has a higher precedence than the addition operator so (2 * 10) will be evaluated first. 



**Concept:** Associativity
```js
var a = 3,
    b = 4,
    c = 5;
console.log (a = b = c); //5
console.log (b); //5 
```
Returns `3`, the assignment operator (`=`) uses right-to-left associativity so firstly b is assigned the value of c which is 5, and then a is assigned the new value of b.



**Concept:** Associativity
```js
var a = 2,
    b = 8,
    c = 5;
console.log(a < b < c); //true
```
Returns `true`. We might expect `false` because b is not smaller than c, however due to the left-to-right associativity of the smaller-than operator (`<`), 
`(a < b)` is evaluated first as `true`. The next step would be to evaluate whether this `true` result is smaller than c. However the value held in c is of the type "number" (`typeOf(c)// "number"`), 
 so the javascript engine will do type coercion on the `true` result which coerces to the number 1 (`Number(true) //1`), so js will be evaluating `1 < 5` to be `true`.






