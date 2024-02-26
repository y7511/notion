# java script arrow function

Arrow functions were introduced in ES6.

Arrow functions allow us to write shorter function syntax:

```html
let myFunction = (a, b) => a * b;
```

**Before Arrow:**

```html
hello = function() {
  return "Hello World!";
}
```

**With Arrow Function**

```html
hello = () => {
  return "Hello World!";
}
```

**Arrow Functions Return Value by Default**

```html
hello = () => "Hello World!";
```

If you have parameters, you pass them inside the parentheses

arrow function with parameters

```html
hello = (val) => "Hello " + val;
```

**Arrow Function Without Parentheses**

In fact, if you have only one parameter, you can skip the parentheses as well

```html
hello = val => "Hello " + val;
```

# What About this?

The handling of `this` is also different in arrow functions compared to regular functions.

In short, with arrow functions there are no binding of `this`.

In regular functions the `this` keyword represented the object that called the function, which could be the window, the document, a button or whatever.

With arrow functions the `this` keyword *always* represents the object that defined the arrow function.

Let us take a look at two examples to understand the difference.

Both examples call a method twice, first when the page loads, and once again when the user clicks a button.

The first example uses a regular function, and the second example uses an arrow function.

The result shows that the first example returns two different objects (window and button), and the second example returns the window object twice, because the window object is the "owner" of the function.

# Example

With a regular function `this` represents the object that *calls* the function:

```html
// Regular Function:
hello = function() {
  document.getElementById("demo").innerHTML += this;
}

// The window object calls the function:
window.addEventListener("load", hello);

// A button object calls the function:
document.getElementById("btn").addEventListener("click", hello);
```

# Example

With an arrow function `this` represents the *owner* of the function:

```html
// Arrow Function:
hello = () => {
  document.getElementById("demo").innerHTML += this;
}

// The window object calls the function:
window.addEventListener("load", hello);

// A button object calls the function:
document.getElementById("btn").addEventListener("click", hello);
```

QUESTION

Deeclare a function fullname and it print out your fullname

```html
const fullname = () => {
  console.log("yordanos awoke");

}
fullname();
```

```html
numbers = [5, 6, 7, 8, 9,]
numbers.forEach(function(value , index , arr1) =>{
counsle.log(arr1)
arr1 arr1 arr1
```