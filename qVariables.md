#Variables and Scope

**Concept** Implied Global; Scope
```js
function doSomething(){
    a = 10;
};
doSomething();
console.log(a); //10
```
Invoking `doSomething()` results in `a` being available in the global scope.  Without the `var` declaration `var a = 10` the variable is implied as global.


**Concept** Hoisting
```js
console.log(a); //"undefined"
var a = 'Hello';
console.log(a); //"Hello"
```
Before `a` is assigned a value it is 'hoisted', which means a space in memory is created for `a`. "undefined" is like a placeholder, or an empty bucket, currently 
holding the "undefined" value.  Hoisting doesn't mean that the js engine moves the declaration to the top of the code, it is simply creating `a` in memory for this given scope.


**Concept** Scope
```js
var a = 5;
function invokeMe(){
    var a = 'fish';
    console.log(a);
}
function doSomething(){
    console.log(a);
    var a = 87;
}
function doSomethingElse(){
    console.log(a);
}

console.log(a); //5 [1]
invokeMe(); //"fish" [2]
console.log(a); //5 [3]
doSomething(); //"undefined" [4]
doSomethingElse(); //5 [5]
```

[1] `a` is  declared and assigned the `"number"` type value of 5 in the global scope. 
[2] invokeMe() creates a new scope and declares the variable `a` to which it assigns the `"string"` value of "fish". 
[3] The `a` in invokeMe scope is not the same as the originally declared `a` which is in global scope so when a is printed again it is still 5
[4] Here the value of a is logged to the console before it is assigned the number value type of 87, however `a` is hoisted so is `undefined` when logged
[5] `a` is not declared in doSomethingElse so the js engine looks to the outer scope for a value and finds 5 in the global scope
