
## Agenda

1. Review: Loops
2. Review: Everything
3. Tutorial: Data Structures Part 1: Arrays
4. Tutorial: Data Structures Part 2: Objects
5. Extra Review Materials

---

## Review: Loops

Questions on loops?
## Review: Questions on _anything_ so far?

Add to [this doc](https://cryptpad.fr/doc/#/2/doc/edit/maTy+shIGct+ggx8iZwkkJa1/)

## Data Structures Part 1: Arrays

### Coding Glossary: Arrays

| Review         |                                                                                          |
| -------------- | ---------------------------------------------------------------------------------------- |
| variable       | name for a placeholder piece of data                                                     |
| declaration    | using `let` to assign a value to a variable or using `function` to create a new function |
| variable types | `boolean`, `number`, `string` (words)                                                    |

| New terms |                                                                             |
| --------- | --------------------------------------------------------------------------- |
| array     | data structure that holds a _series_ of variables, uses `[]`, order matters |
| element   | one piece of array data                                                     |
| index     | location of a particular element, starting at index of 0                    |
| property  | a value we are accessing, using the `.` syntax                              |

### Declaring an **_Array_**

Array is a variable type. Arrays are a *list* of data written with square brackets (`[]`). 

Arrays are living variables, so you can change the value of them over time.

```js
let myNewArray = [];
```

### Initializing an array with **_Elements_**

An element is an item that exists inside of an array. 

```js
let myNewArray = [10, 15, 20];
```

### Retrieving a specific **_Element_** with the **_Index_**

The index is the location of the data we want to grab. The location is automatically assigned because of the `array`, since it is a _series_ of data.

Arrays start counting 0 and increases by one for every element. You can think of this as "How far is the element I am trying to get *away* from the starting element".

To access elements in an array, we use the array name + `[]`

```js
let myNewArray = [10, 15, 20];

myNewArray[0]; // 10
myNewArray[1]; // 15
myNewArray[2]; // 20
```

### Arrays are like tables

<table>
<tbody>
<tr><td>index</td><td>0</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td>value</td><td>"this"</td><td>"is"</td><td>"a"</td><td>"sentence"</td></tr>
</tbody>
</table>

```js
let data = ['this', 'is', 'a', 'sentence'];
```

In code, we typically only want an array to hold 1 type of data. So it should be _either_ a list of numbers, booleans, or strings.

### Array properties

Properties are variables that are unique to an object (in this instance an array). We again use the `.` to reference a specific property we want to access.

Arrays have a property called [`length`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/length). This gives us how many items exist in the array.

```js
let myArray = [2, 4, 6]; // 3 items total
myArray.length; // this is 3
```

This counts the number of **_elements_** that exist inside the array.

### Adding to Arrays

We can change the value of an element in the array by reassigning it, like we do with normal variables.

```js
let teachers = ['Sam', 'Patrick', 'Rory'];
teachers[1] = 'Sam';
// override the old value, reassign to new
// teachers is now ["Sam", "Sam", "Rory"]
```

If we use an index (location), that does not exist yet, it will add empty `undefined` items in the series until it gets to that location.

```js
let animals = ['Cat', 'Dog']; // animals has elements at 0 and 1
animals[4] = 'Giraffe';
// animals is now ["Cat", "Dog", undefined, undefined, "Giraffe"]
```

This isn't the best way to add to an array, because we don't want to accidentally create empty variables.

### Unique Attributes of an Array

Arrays have special functionality, along with their properties, that allow us to enact actions on them. These actions are *functions*, but they need to *reference the array they will be acted on*. 

#### `.push()`

`push()` is a function we have seen inside of p5, but [`.push()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push) is a function that exists in an array. We need to use the name of our array, and the `.` to use the specific function.

```js
let myArray = [2, 4, 6];
myArray.push(8);
// this automatically adds 8 to the end of the array
// the new array is [2, 4, 6, 8]
```

This adds an element to the end of the array.

**Note**: This is different from p5's `push()` method. p5 has redefined `push()`/`pop()` to store states. `.push()` has different syntax and _must_ be used _on_ an array. So anytime we see the prepending `.`, it likely means it needs to be used on an object.

#### `.splice()`

To remove elements in an array, we use [`.splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice). 

```js
// splice(start, deleteCount) 
// it takes where you want to start and how many elements you want to remove
let evenNumbers = [2, 4, 6, 8, 10] 
evenNumbers.splice(3, 1) // removes 8
// the new array is [2, 4, 6, 10]
```

### Arrays and Loops

Typically it is very cumbersome to access every element inside of a loop every time. Given an array:

```js
let pets = ['dog', 'cat', 'hamster', 'giraffe', 'horse'];
```

If we want to use or reference any one of these we would need to do something like:

```js
print(pets[0]); // prints: dog
print(pets[1]); // prints: cat
print(pets[2]); // prints: hamster
print(pets[3]); // prints: giraffe
print(pets[4]); // prints: horse
```

But, we already see a pattern of a number increasing every time. So, using the attributes we know so far, we can go through the loop. We already know our end condition, because it is the number of elements in our loop. So we could write:

```js
for (let count = 0; count < 5; count++) {
	print(pets[count]);
}
```

But, our end condition might be malleable, or we might add another pet later on. So we can use the property `.length` instead of hard-coded 5.

```js
// instead of count < 5, make it dynamic using pets.length
for (let count = 0; count < pets.length; count++) {
	print(pets[count]);
}
```

If we wanted to make it clearer, we could declare a local variable:

```js
for (let count = 0; count < pets.length; count++) {
	// setting a local variable in case we want to use pets[count] again
	let currentPet = pets[count];
	print(currentPet);
}
```

There is a shorthand for this! If we don't need to know the number, we can automatically create and assign `currentPet`:

```js
// shorthand for above example
for (let currentPet of pets) {
	print(currentPet);
}
```

This is a special loop _just for arrays_, that is shorthand for assigning a variable to the index of the current iteration.

## Data Structures Part 2: Objects

An object is a data structure similar to an array, but instead of using `[]`, it uses `{}`. It also is useful when we need unordered data, *or we need to store multiple data types in one variable.*

| New terms |                                                                                        |
| --------- | -------------------------------------------------------------------------------------- |
| object    | data structure that holds variables using key-value pairs, uses `{}`, it is unordered. |
| key       | the `property` we access when we want to retrieve a piece of data from the object.     |
| value     | similar to the `element` in an array, the data that is stored                          |
### Declaring an **_Object_**

An Object is a variable type. Objects are an *unordered list* of data written with curly braces (`{}`). 

```js
let myNewObject = {};
```

### Initializing an array with **_Values_**

The main difference between objects and arrays is that arrays can only store *one* data type, but objects can hold multiple ones. 

```js
let myPet = {
	name: "Oreo",
	age: 13,
	isCat: true
}
```

### Retrieving a specific **_Value_** with the **_Property_**

Unlike arrays, objects are unordered. But, we can access the named property to retrieve which piece of data we want. 

To access values in an object, we use the object name + `.` + property name

```js
let myPet = {
	name: "Oreo",
	age: 13,
	isCat: true
}

// object name + . + property name
// myPet.name
// myPet.age
// myPet.isCat
print(`${myPet.name}`) // prints "Oreo"
```

### Unique Attributes of an Object

We can add new `properties` by simply using a new property name. 

```js
let triangle = {
    a: 10,
    b: 15
}
triangle.c = 20
// this automatically adds .c as an accessible property
// the new object is {a:10, b:15, c:20}
```
### Objects and Loops

Just like with arrays, objects also have a special loop.

```js
const object = { a: 1, b: 2, c: 3 };

for (const property in object) {
  console.log(`${property}: ${object[property]}`);
}

// Expected output:
// "a: 1"
// "b: 2"
// "c: 3"
```

## And that's it!

We know everything about JavaScript! 

...For now. But generally this is the syntax we will be building on for the rest of the semester. After Project #3, we will focus much more heavily on why p5.js is a cool tool. You can review the class notes, or also check out [this JavaScript cheatsheet](https://samheckle.github.io/how-to/write-javascript) for quick references on things you should know about JavaScript. There are some things we did not cover (like different syntax for functions), but most everything else is applicable to your Project #3.

---

## Extra Review Materials
### Review Videos

- Coding Train[7.1 What is an array?](https://www.youtube.com/watch?v=VIQoUghHSxU)
- Coding Train [7.2 Arrays and loops](https://www.youtube.com/watch?v=RXWO3mFuW-I)
- Coding Train [7.3: Arrays and Objects](https://thecodingtrain.com/tracks/code-programming-with-p5-js/code/7-arrays/3-arrays-objects)

### Review Documentation (these are textbook definitions)

- MDN [for...of](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of) loops with arrays
- MDN [array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- MDN [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
