### Find out if a variable is an Array

In JavaScript an Array instance is actually an object. So if you do something like below, it does not clearly tell you if its an array

```js
var arr = [1,2,3,4];
typeof arr; //'object'
```

So how do you find if the variable is an array?

```js
var arr = [1,2,3,4];
arr.constructor === Array //true if array variable
```

or, you can also go by the constructor name
```js
arr.constructor.name === 'Array' //true if array variable
```