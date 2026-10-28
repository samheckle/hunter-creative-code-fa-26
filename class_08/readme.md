# Week 08

## Agenda

1. Reading Discussion #2
2. Tutorial: Data Structures Part 2: Objects
3. Tutorial: p5.js Sound
4. Extra Review Materials

## Reading Discussion #2

Take notes in the document in Brightspace.

- How are you currently using AI? Do you use AI in your artistic processes now?
- What are the different approaches you might take in using AI in the future (if you will)?
- Can technology be biased? Or is it designed that way?
- When you were younger, how did you imagine your adult life? What did you imagine yourself doing? Has AI changed that?
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


## Tutorial: p5.js Sound

To use sound in p5, we use the [p5 sound library](https://p5js.org/reference/p5.sound/), which allows us to add, manipulate, and create sound with p5.

### Sources for sound:

- [orchestral sample library](http://virtualplaying.com/virtual-playing-orchestra/)
- [free music archive](https://freemusicarchive.org/)
- [freesoundorg](https://freesound.org/)
- [bbc sound effects](http://bbcsfx.acropolis.org.uk/)
- [free sound picture](https://www.soundofpicture.com/)

### Sound Project references

- https://teropa.info/loop/#/title
- https://www.nytimes.com/interactive/2018/09/21/magazine/voyages-travel-sounds-from-the-world.html
- http://jazz.computer/
- https://patatap.com/
- https://youtu.be/HI1raqxrUdk?si=j01yIjgDCCW91PpI
  - cassie's [sketch](https://editor.p5js.org/cassie/sketches/YZHxZ9ffl) recreating it

## Extra Review Materials
### Review Videos

- Coding Train [7.3: Arrays and Objects](https://thecodingtrain.com/tracks/code-programming-with-p5-js/code/7-arrays/3-arrays-objects)
* [17.1: Loading and Playing sound](https://youtu.be/Pn1g1wjxl_0?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.3: Timing, Jumps and Cues](https://youtu.be/SfA5CghXw18?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.4: Amplitude Analysis](https://youtu.be/NCCHQwNAN6Y?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.5: Adding Sound Effects - video tutorial](https://youtu.be/40Me1-yAtTc?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.6: Sound Synthesis - video tutorial](https://youtu.be/Bk8rLzzSink?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.8: Microphone Input](https://youtu.be/wUSva_BnedA?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.9: Sound Visualization: Graphing Amplitude](https://youtu.be/jEwAMgcCgOA?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.10: Sound Visualization: Radial Graph](https://youtu.be/h_aTgOl9J5I?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
* [17.11: Sound Visualization: Frequency Analysis with FFT](https://www.youtube.com/watch?v=2O3nm0Nvbi4&list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jp

### Review Documentation (these are textbook definitions)

- MDN [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)