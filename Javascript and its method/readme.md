# What is an Array?

**In JavaScript,** `Array` **is a built-in global object that allows you to store multiple elements at once.**

# Declaration syntax of Array

```javascript
const arr = ["Apple" ,"Banana" , "Orange"];
console.log(arr);
```

# JavaScript Array Methods

## 1\. JavaScript Array length

In this tutorial, we will learn about the JavaScript Array length property with the help of examples.

```javascript
let city = ["California", "Barcelona", "Paris", "Kathmandu"];

// find the length of the city array
let len = city.length;
console.log(len);

// Output: 4
```

### length Syntax :

```javascript
arr.length
```

## 2\. JavaScript Array reverse()

> In this tutorial, you will learn about the JavaScript Array reverse() method with the help of examples.
> 
> **The** `reverse()` **method returns the array in reverse order.**
> 
> ```javascript
> let numbers = [1, 2, 3, 4, 5];
> 
> // reversing the numbers array
> let reversedArray = numbers.reverse();
> 
> console.log(reversedArray);
> 
> // Output: [ 5, 4, 3, 2, 1 ]
> ```

### reverse() Syntax :

```javascript
arr.reverse()
```

## **3\. JavaScript Array sort()**

> In this tutorial, we will learn about the JavaScript Array sort() method with the help of examples.
> 
> The `sort()` method sorts the items of an array in a specific order (ascending or descending).
> 
> ### **Example:**
> 
> ```javascript
> let city = ["California", "Barcelona", "Paris", "Kathmandu"];
> 
> // sort the city array in ascending order
> let sortedArray = city.sort();
> console.log(sortedArray);
> 
> // Output: [ 'Barcelona', 'California', 'Kathmandu', 'Paris' ]
> ```

### sort() Syntax

```javascript
arr.sort(compareFunction)
```

## **4\. JavaScript Array fill()**

In this tutorial, we will learn about the JavasScript Array fill() method with the help of examples.

> The `fill()` method returns an array by filling all elements with a specified value.
> 
> ### **Example:**
> 
> ```javascript
> // defining an array 
> let fruits = ['Apple', 'Banana', 'Grape'];
> 
> // filling every element of the array with 'Cherry'
> fruits.fill("Cherry");
> 
> console.log(fruits);
> 
> // Output: 
> // [ 'Cherry', 'Cherry', 'Cherry' ]
> ```

fill() Syntax

```javascript
arr.fill(value, start, end)
```

## 5\. Javascript Array join()

> In this tutorial, we will learn about the JavaScript Array join() method with the help of examples.
> 
> The `join()` method returns a new string by concatenating all of the elements in an array, separated by a specified separator.
> 
> ### **Example:**
> 
> ```javascript
> let message = ["JavaScript", "is", "fun."];
> 
> // join all elements of array using space
> let joinedMessage = message.join(" ");
> console.log(joinedMessage);
> 
> // Output: JavaScript is fun.
> ```

## **6\. Javascript Array toString()**

> In this tutorial, you will learn about the JavaScript Array toString() method with the help of examples.
> 
> The `toString()` method returns a string formed by the elements of the given array.
> 
> ```javascript
> // defining an array
> let items = ["JavaScript", 1, "a", 3];
> 
> // returns a string with elements of the array separated by commas
> let itemsString = items.toString();
> 
> console.log(itemsString);
> 
> // Output: 
> // JavaScript,1,a,3
> ```

### toString() Syntax

```javascript
arr.toString()
```

## 7\. JavaScript Array pop()

> In this tutorial, we will learn about the JavaScript Array push() method with the help of examples.
> 
> The `pop()` method removes the last element from an array and returns that element.
> 
> ### **Example:**
> 
> ```javascript
> let cities = ["Madrid", "New York", "Kathmandu", "Paris"];
> 
> // remove the last element
> let removedCity = cities.pop();
> 
> console.log(cities)         // ["Madrid", "New York", "Kathmandu"]
> console.log(removedCity);   // Paris
> ```

### pop() Syntax:

```javascript
arr.pop()
```

## 8\. JavaScript Array push()

> In this tutorial, we will learn about the JavaScript Array push() method with the help of examples.
> 
> The `push()` method adds zero or more elements to the end of the array.
> 
> ### **Example:**
> 
> ```javascript
> let city = ["New York", "Madrid", "Kathmandu"];
> 
> // add "London" to the array
> city.push("London");
> 
> console.log(city);
> 
> // Output: [ 'New York', 'Madrid', 'Kathmandu', 'London' ]
> ```

### push() Syntax

```javascript
arr.push(element1, element2, ..., elementN)
```

# Resources:

[Array](https://www.programiz.com/javascript/library/array)