### Find out if an Object is empty

An object is considered empty when it does not have any attributes in it. For eg. any properties or methods. How do you find if an object is empty?

```js
var obj = {};
var keysArr = Object.keys(obj);
if(keysArr.length === 0) {
    //empty
} else {
    //non empty
}
```
Browser Support: Its supported in all major browsers and also NodeJS
Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys