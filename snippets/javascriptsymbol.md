### What is a JavaScrit Symbol type?

JavaScript has a new primitive data type called Symbol() that was added in the ES6 spec. 

#### What is a Symbol?
As per the definition a Symbol is a unique and immutable identifier.

```js
var s = Symbol('description about the symbol');

eg.
var empID = Symbol('employee id');
var name = Symbol('name');
```

Symbols are meant to be unique. Even if we create two Symbols with same description, they are not equal.

```js
var s1 = Symbol('s');
var s2 = Symbol('s');
alert(s1 === s2); //false
```

#### Usage
Symbols are most useful when used for object properties or rather when you want to make unique object properties.

```js
var s1 = Symbol('prop'); 
var s2 = Symbol('prop'); //two symbols with same description called prop

//lets use them as our object keys
var obj = {
    s1: 'value1',
    s2: 'value2'
}

alert(obj.s1); //'value1'
alert(obj.s2); //'value2'
```

Normally if you have the same key name for multiple object properties it gets overwritten

```js
var obj = {
    prop: 'value1',
    prop: 'value2'
};

aler(obj.prop); //'value2'
```

Alright then, I hope you have some information now. Go ahead and try it.