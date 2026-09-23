# Week 4

## Agenda

1. Housekeeping
2. Homework Share
3. Lecture: Repetition and Functions
4. On Code Order
5. Extra Review Materials

## Housekeeping

1. Reading #1 due next class
## Homework Share

In breakout rooms, share your projects and try to answer any questions you might have had issues with! We will share in groups for ~10-15 minutes, then come together as a class and look through everyone's work. Each group will select one person to share.

## Repetition and Functions

### Coding Glossary: Review

<table>
<tbody>
<tr><td>function</td><td>

an instruction or command, may or may not have parameters. also known as `method`

</td></tr>
<tr><td>parameters</td><td>

values that are passed into the function inside the `()`. also known as `arguments`.

</td></tr>

<tr><td>declaration</td><td>

using the keyword `let`, names and creates a variable

</td></tr>
</tbody>
</table>

Declarations can also be used for functions, using the keyword `function`

Functions need to be written **_outside_** the `setup()` and the `draw()`

We have already seen an example of this:

```js
function setup() {
  createCanvas(400, 400);
}
function draw() {
	// loops once every frame
}
```

`setup()` and `draw()` are functions that use the function keyword. We have also seen:

```js
function mousePressed() {
  // do something when the mouse is clicked
}
```

### Loading Assets

In order to load assets into a sketch, we can use the keywords `async` and `await` in the `setup` function declaration.

Each asset requires 3 steps:

1. A global variable to store the reference to the asset file
2. `async` in `setup` function declaration + `await` to load the asset file
3. Using the asset as needed in the code

```js
// step 1
let img

// step 2
async function setup() {
  	img = await loadImage("./my-image.png");
  	createCanvas(400, 400);
}

function draw(){
	// step 3
	image(img, 0, 0)
}
```

See [`async_await`](https://p5js.org/reference/p5/async_await/)

### Custom Functions

So far, we have used functions that have only been defined by p5. Even though we are declaring and using `setup()`, `draw()`, and `mousePressed()`, they aren't something we are specifically defining. So, we can [create our own functions](https://p5js.org/reference/p5/function/) too. These still need to be written **_after_** the `draw()`

```js
function myCoolNewFunction() {}
```

We can also make custom parameters:

```js
function myCoolNewFunction(myCoolParameter) {
  print(myCoolParameter);
}
```

#### Coding Glossary: Custom Functions

<table>
<tbody>
<tr><td>declaration</td><td>

using the keyword `function`, names and creates a function

</td></tr>
<tr><td>call</td><td>

to use a function elsewhere in the code

</td></tr>
<tr><td>passing arguments</td><td>

a custom function accepting inputs in their headers, which creates a local placeholder for the data that is received

</td></tr>
</tbody>
</table>

#### Why make custom functions?

1. Code can be duplicated more easily.
2. It makes our code more readable and organized, just like variables.
   - if you notice you are doing the same section of code multiple times, it can probably be a function!

![functions vs var](https://github.com/samheckle/code-toolkit-fa-25/raw/main/images/week_04/functionvar.png)

## On Code Order

We have seen a lot of code, but typically it follows an order. This is the order we use for this class:

1. Global Variables
2. `setup`
3. `draw`
4. Event Functions (like `mousePressed`)
5. Helper Functions (or functions you write yourself)

---
## Review Videos

If you struggled with any of the material this week, please review these coding train videos!

- [5.1 - function basics](https://thecodingtrain.com/tracks/code-programming-with-p5-js/code/5-functions/1-basics)
- [5.2 - parameters and arguments](https://thecodingtrain.com/tracks/code-programming-with-p5-js/code/5-functions/2-arguments)
- p5 Tutorial: [Organizing Code through Functions](https://p5js.org/tutorials/organizing-code-with-functions/)
