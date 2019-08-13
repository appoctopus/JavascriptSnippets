### Add an element to an array

Lets see different ways of adding elements to an array.

* array push()
You can add items to the end of the array. 
```js
var arr = [1,2,3];
arr.push(4);
console.log(arr); //[1,2,3,4]
```

* Direct assignment
```js
var arr = [1,2,3];
arr[arr.length] = 4;
console.log(arr); //[1,2,3,4]
```

* array unshift()
You can add items to the beginnning of an array
```js
var arr = [1,2,3];
arr.unshift(0);
console.log(arr); //[0,1,2,3]
```

* array splice()
Using splice method you can specify where you want to add items. Ref: 
```js
var arr = [1,2,3];
arr.splice(2, 0, 9); //(start_index, number_of_items_to_remove, item/items_to_insert)
console.log(arr); //[1,2,9,3]

//add multiple items
arr.splice(2, 0, 9, 8, 7);
console.log(arr); //[1,2,9,8,7,3]
```

All these techniques discussed above modifies the original array. The one below does not.

* array concat()
Add items to the end of an array. Does not modify the original array
```js
var arr = [1,2,3];
arr.concat(9); //[1,2,3,9]
console.log(arr); //[1,2,3]

//you can also pass an array itself
arr.concat([5,6]); //[1,2,3,5,6]
console.log(arr); //[1,2,3]
```

Well, try to experiment with all these techniques. I am sure you will discover more.
