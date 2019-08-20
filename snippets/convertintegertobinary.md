### Convert integer number to binary

JavaScript has a built in way of converting integer numbers to binary (i.e 0's & 1's). Lets find out how.

```js
var num = 1234;
var binaryString = num.toString(2); //"10011010010"
```

toString() method takes an argument which is the radix. 2 is for binary. Similarly 16 is for hexadecimal. Default is 10.

```js
var num = 255;
num.toString(16); //"ff"

var num = 255;
num.toString(); //"255"

var num = 255;
num.toString(10); //"255"
```
What happens when you have a floating number? Give it a try :)
Read more: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toString
