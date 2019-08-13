### Copy an object by value

By using the ES6 spread operator we can copy an object by value very easily.

```js
var obj = {
  a: 1, 
  b:2
}
var copy = { ...obj }; //{a: 1, b: 2}
```

Now modifying copy's attributes will not modify our original object.

Learn more about ES6 spread operator here: https://codeburst.io/a-simple-guide-to-destructuring-and-es6-spread-operator-e02212af5831
