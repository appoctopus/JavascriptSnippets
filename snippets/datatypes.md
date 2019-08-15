### Data Types in JavaScript
When we declare a variable in JavaScript we don't declare its type. But there are data types that work behind the scenes although JavaScript is a Dynamically Typed Language. 

There are 7 types in JavaScript and we can divide them into two kinds.
* Primitive
* Every thing else is Objects

Primitive Data Types are number, boolean, string, undefined, null, symbol(introduced in ES6)

```js
var n = 12;
typeof n; //"number"
n instanceof Object; //false

var s = "hello";
typeof s; //"string"

var b = true;
typeof b; //"boolean"

typeof undefined; //"undefined"

typeof null; //"object"

var sym = Symbol('a');
typeof sym; //"symbol"
```

Rest all are objects for eg. Array, RegExp, Functions, Objects etc.

```js
var arr = [];
typeof arr; //"object"
arr instanceof Object; //true

var f = function() {};
typeof f; //"function"
f instanceof Object; //true
```

Explore more...
