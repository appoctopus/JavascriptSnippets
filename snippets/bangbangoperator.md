### Bang Bang Operator !!

Smart little trick to convert any JS value to its Boolean equivalent and know if its true or false

```js
!! 0 //false
!! { } //true
!! null //false
!! undefined //false
!! "hello" //true
!! false //false
!!true //true
```