### The void operator

Did you know that JavaScript has a void operator just to explicitly return undefined. Its a unary operator, meaning only one
operand can be used with it. You can use it like shown below - standalone or with a parenthesis.

```js
void expression;
void(expression);
```

```js
void 0; //returns undefined
void(1); //returns undefined

void 'hello'; //undefined
void {}; //undefined
void []; //undefined

void myFunction(); 
void(myFunction());
```

#### But why?
Why the hell do you need a special keyword just to return undefined instead of just returning undefined? 
Well, the reason is before ES5 you could actually assign a new value to the original undefined like so
undefined = "js snippet", and most browsers would support it. 
So as to return the original undefined and just to be double sure the void operator was used. 

Some examples,

```js
//just a normal function
function test() {
    console.log('hello');
    return 2;
}
//lets call it
test(); //output is hello followed by 2

//now lets try with void
void test(); //output is hello followed by undefined
```
So in the example above, void cancels the return from the function and explicitly returns undefined. But the log is anyways printed.

Give it a try, would you!!
