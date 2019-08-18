### Enhance/Augment native JavaScript objects using prototypes

Ever wandered if there is a way to augment native JS objects. Well it is possible. For eg. you want to write your own string reverse() method that can be used by all strings. We can use the prototype property to augment additional functionality.

Every string variable/literal that you create is an instance of the String constructor function
```js
var s = "hello";
s instanceof String; //true
```

Every Function or a constructor function that you create gets a prototype property which can be used to augment additional functionality.

```js
if(!String.prototype.reverse && typeof String.prototype.reverse !== 'function') {
    String.prototype.reverse = function() {
        //this is the instance of the string data with which you will call the reverse method. 
        return this.split('').reverse().join('');
    }
}

//from now on every string that you create will have the reverse method.
var s = "hello";
s.reverse(); //

var s1 = 'how are you?'
s1.reverse(); //

"good morning".reverse(); //
```


Explore more about the prototype property. There is a lot that happens around it. 
