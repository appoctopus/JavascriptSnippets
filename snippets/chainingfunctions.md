### Chaining functions in JavaScript

You can chain function calls when using Constructor functions and return the object instance from inside the methods that you have defined. 

Bit too much is it. Lol! Well its simple, Let's call our Constructor function as Class (bascially thats how you declare a class in JavaScript before ES6 classes). Now the whole idea is that if you return "this" from inside the functions that you have defined within your class, you can chain them while calling. 

```js

//Define your constructor function
function Employee() {
    this.setName = function(name) {
        this.name = name;
        return this; //this does the chaining trick
    }
    this.print = function() {
        console.log('Employee name is: ', this.name);
    }
}

//now create an instance and call the methods using chaining
var e = new Employee();
e.setName('John Doe').print(); //Employee name is: John Doe

```
You can keep going with chaining...

Constructor functions are concepts of Object Oriented JavaScript and is a very interesting subject in itself. Go get experimenting with it..
