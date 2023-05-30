# What is a function?

> A JavaScript function is a block of code designed to perform a particular task.
> 
> A JavaScript function is executed when "something" invokes it (calls it).
> 
> **Example:**
> 
> ```javascript
> // Function to compute the product of p1 and p2
> function myFunction(a1, a2) {
>   return a1 * a2;
> }
> ```

# Syntax

> A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.
> 
> The code to be executed, by the function, is placed inside curly brackets: **{}**
> 
> ```javascript
> function name(parameter1, parameter2, parameter3) {
>   // code to be executed
> }
> ```
> 
> Function **parameters** are listed inside the parentheses () in the function definition.
> 
> Function **arguments** are the **values** received by the function when it is invoked.
> 
> Inside the function, the arguments (the parameters) behave as local variables.

# Why Functions?

> You can reuse code: Define the code once, and use it many times.
> 
> You can use the same code many times with different arguments, to produce different results.
> 
> ### Example:
> 
> ```javascript
> function toCelsius(fahrenheit) {
>   return (5/9) * (fahrenheit-32);
> }
> document.getElementById("demo").innerHTML = toCelsius(77);
> ```

# Different ways of writing functions in JavaScript

* There are 3 ways of writing a function in JavaScript:
    
    * **Function Declaration**
        
    * **Function Expression**
        
    * **Arrow Function**
        

> **Function Declaration:** Function Declaration is the traditional way to define a function. It is somehow similar to the way we define a function in other programming languages. We start declaring using the keyword *“function”.* Then we write the function name and the parameters.
> 
> **Example:**
> 
> ```javascript
> 
> 	// Function declaration
> 	function add(a, b) {		
> 		console.log(a + b);
> 	}
> 	
> 	// Calling a function
> 	add(2, 3);
> // Output: 5 
> ```
> 
> **Function Expression:** Function Expression is another way to define a function in JavaScript. Here we define a function using a variable and store the returned value in that **variable**.
> 
> ```javascript
> 
> 	// Function Expression
> 	const add = function(a, b) {
> 		console.log(a+b);
> 	}
> 	
> 	// Calling function
> 	add(2, 3);
> // Output:5
> ```
> 
> [**Arrow Functions**](https://www.geeksforgeeks.org/arrow-functions-in-javascript/)**:** Arrow functions are been introduced in the **ES6 version** of JavaScript. It is used to shorten the code. Here we do not use the “**function”** keyword and use the arrow symbol.
> 
> **Example:** Below is the example that illustrates the use of the *Arrow* *Function.*
> 
> ```javascript
> 
> 	let add = (a, b) => a + b;
> 	
> 	console.log(add(3, 2));
> ```

# Resources:

[JavScript Functions](https://www.w3schools.com/js/js_functions.asp)