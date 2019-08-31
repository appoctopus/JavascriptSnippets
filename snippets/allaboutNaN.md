### All about NaN (Not a Number)

NaN stands for Not a Number. Its a special value in JavaScript that depicts a non number. But when do you encounter one?

Well, whenever you are doing an arithmatic operation in JavaScript and you are passing a non number by mistake or intentionally you will get a NaN as output.

```js
12*"a"         => NaN
12/"abc"       => NaN
(12 + 3) / {}  => NaN
12 - "a"       => NaN
12 + "a"       => "12a"
```
In the examples above the arithmatic operations are expecting numbers but you passed a string or anything non numerical. Rather than throwing a runtime error, JavaScript gives a NaN. However, the plus symbol which is also used for concatenation actually joins the two and gives a combined string. Thats an exception :)

But do remember, number like strings are converted to number behind the scenes. So you dont get a NaN here. For eg.

```js
12 * "5" => 60
12/"6"   => 2
12 - "5" => 7
```

#### Things to note
* NaN === NaN //false
* typeof NaN === 'number'
* NaN is false by default. (!!NaN => false)

How to find? 
Use the isNaN() global function to look for NaN values. Examples below,

```js
isNaN(12 * "a"); //true

isNaN(12 * "5"); //false (converted to number behind the scenes)

isNaN(12); //false (because it is not a NaN, its a proper number)

isNaN(NaN); //true

isNaN("a"); //true 

isNaN("12"); //false (converted to number behind the scenes)
```
I hope now you have enough ammunitions to give it a try!!

