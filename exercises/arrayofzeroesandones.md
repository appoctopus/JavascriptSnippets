### Order an array of random 0's & 1's

Given array of random 0's and 1's. Put them in sequential order of 0's followed by 1's.
```js
Input: [1,0,1,1,1,0,0,1,0,1,0]
Output: [0,0,0,0,0,1,1,1,1,1,1]
```
#### Solution
```js
function order(arr) {
    //first count the number of 0's in the array
    var count = 0,
        arrLength = arr.length,
        newArr = [];
    for(var i = 0; i < arrLength; i++) {
        arr[i] === 0 && count++;
    }
    //now fill the new array with the number of counted 0's.
    for(var i = 0; i < count; i++) {
        newArr.push(0);
    }
    //fill the rest of the length with 1's
    for(var i = count; i < arrLength; i++) {
        newArr.push(1);
    }
    return newArr;
}

order([1,0,1,1,1,0,0,1,0,1,0]); //[0,0,0,0,0,1,1,1,1,1,1]
```
