### What is functional programming?

using functions to the best effect for creating clean and maintainable software

-----------

### What is a pure function and how do we know if something is a pure function?

The function always returns the same result if the same arguments are passed in

EX :

```
var tax = 20;
function calculateTax(productPrice) {
  return productPrice * (tax / 100) + productPrice;
}

```

A pure function can not depend on outside variables. It fails one of the requirements thus this function is impure.

----------

### What are the benefits of a pure function?

They’re easier to reason about They’re easier to combine They’re easier to test They’re easier to debug They’re easier to parallelize

--------

### What is immutability?

Immutable data cannot change its structure or the data in it. It’s setting a value on a variable that cannot change, making that value a fact, or sort of like a source of truth

-------

### What is Referential transparency?

In programming, referential transparency applies to programs. As programs are composed of subprograms, which are programs themselves, it applies to those subprograms, too. Subprograms may be represented, among other things, by methods. That means method can be referentially transparent

-------------

### What is a module?

Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

--------------
### What does the word ‘require’ do?

require() is not part of the standard JavaScript API. But in Node.js, it's a built-in function with a special purpose: to load modules.


------------
How do we bring another module into the file the we are working in?


```
module.exports = {
    sum: function(a,b) {
        return a+b
    },
    multiply: function(a,b) {
        return a*b
    }
};
Main js file

// File app.js
var tools = require("./cal.js");
var value = tools.sum(10,20);
console.log("Value: "+value);
Console Output

Value: 30
```

What do we have to do to make a module available

Download & install Node.js Create a Node project Write your module :There should now be a package.json file inside your project directory. We need to write our code to upload it as a module.


### Things I want to know more about

I want to know more about overall backend and servers using node js

