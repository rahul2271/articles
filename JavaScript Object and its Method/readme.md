# What is Object in JavaScript?

> In JavaScript, objects are king. If you understand objects, you understand JavaScript.

In JavaScript, almost "**everything**" is an object.

* Booleans can be objects (if defined with the `new` keyword)
    
* Numbers can be objects (if defined with the `new` keyword)
    
* Strings can be objects (if defined with the `new` keyword)
    
* Dates are always objects
    
* Maths are always objects
    
* Regular expressions are always objects
    
* Arrays are always objects
    
* Functions are always objects
    
* Objects are always objects
    

All JavaScript values, except primitives, are objects

## Syntax

```javascript
const person = {
        firstName:"John",
        lastName:"Doe", 
        age:50, 
        eyeColor:"blue"
};
```

# JavaScript Object Methods

JavaScript methods are actions that can be performed on objects.

A JavaScript **method** is a property containing a **function definition**.

| **Property** | **Value** |
| --- | --- |
| firstName | John |
| lastName | Doe |
| age | 50 |
| eyeColor | blue |

## Accessing Object Methods

You access an object method with the following syntax:

```javascript
objectName.methodName()
```

### Example :

```javascript
name = person.fullName();
```

## Adding a Method to an Object

```javascript
person.name = function () {
  return this.firstName + " " + this.lastName;
};
```

## Using Built-In Methods

This example uses the `toUpperCase()` method of the String object, to convert a text to uppercase:

```javascript
let message = "Hello world!";
let x = message.toUpperCase();
//Output :  HELLO WORLD!
```

# Resources :

[w3school](https://www.w3schools.com/js/js_object_methods.asp)