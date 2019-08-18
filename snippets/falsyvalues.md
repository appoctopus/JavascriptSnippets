### Falsy values in JavaScript

In JavaScript the following values are false by default

* undefined
* null
* false
* 0
* '' (empty string)
* NaN

Rest everything is true. Even an empty object, array etc.

How to find? 
Well we can use the !! (double negation operator) to find the boolean equivalent of a value

```js
var a = null;
!!a; //false

var b = {};
!!b; //true

var c = NaN;
!!c; //false

var d = '';
!!d; //false

!!0; //false
```
