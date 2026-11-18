# Week 12

1. Housekeeping
2. Reading Discussion #4
3. Tutorial: Webcam
4. Tutorial: External Libraries
5. Extra Review Materials

## Housekeeping

1. Attendance
2. No class next week - Thanksgiving
3. Project #5 Research & Proposal in 2 weeks

## Reading Discussion #4

## Tutorial: Webcam

We can leverage the webcam to do a lot of things inside p5.js, and we can even manipulate individual pixels.

Let's start with regular pixel manipulation and then add a library on top of it.

The most important line of code for video allows us to enable webcam usage.

```js
// prompts the browser to use the webcam
webcam = createCapture(VIDEO);
```

We could _also_ use a phone camera instead if we wanted

```js
// if i am using a phone camera
let constraints = {
	audio: false,
	// back camera code
	video: {
		facingMode: {
			exact: 'environment', // back camera
		},
	},
	// front camera code
	//video: {
	//facingMode: "user"
	//}
};
webcam = createCapture(constraints);
```

What this does is allow us to add the webcam as an HTML element. If we wanted to hide that element and just display the camera on the screen, we could write

```js
//... in the setup
webcam.hide();
//... in the draw
// display webcam data to the draw
image(webcam, 0, 0);
```

## Tutorial: External Libraries

p5.js and p5.sound.js are two core frameworks that we have used in this class that focus on graphic and sound explorations in the web. But, we can also use _external_, meaning not maintained by the Processing Foundation, libraries that leverage p5 to do interesting things.

We can see a full list of the libraries of p5 by visiting https://p5js.org/libraries/directory/

For your final project, you will pick a library to research and teach the class through a short demo that you will build. Each presentation will cover:

1. what the library does and how it might be used in real world
2. how the library works
3. short demo on the library

Each presentation should be ~10 minutes long, including the demo. _Your demo must differ from any examples given by the library themselves_.

There are lots of interesting things to explore here:

- 3D (I would also look at the WebGL tutorials: https://p5js.org/tutorials/)
- [p5 riso](https://antiboredom.github.io/p5.riso/) if you wanted to make it physical
- [p5 glitch](https://ffd8.github.io/p5.glitch/)
- continue with advanced p5.sound library
- look into other functionality of p5.js that may not have been covered in class

Good benchmarks for choosing a library to work with:

- What does the documentation look like?
- Is it well-supported by the p5 community? When was the last time the library was updated?
- Are there a lot of tutorials using the library?
- Is it an interesting topic to you?


### Example Library: Using ml5

https://ml5js.org/ is a library built on top of p5 to use machine learning. They have a few different types of tools that you are welcome to use, but today's demo will focus on BodyPose https://docs.ml5js.org/#/reference/bodypose

The first thing we always do when using an external library is open up our `index.html` and import the library code.

```html
<script src="https://unpkg.com/ml5@1/dist/ml5.js"></script>
```

### Example Library: Using p5.glitch

https://ffd8.github.io/p5.glitch/ allows you to directly manipulate the binary data of a sketch to create a glitch effect. 

We can import it by using

```html
<script src="https://cdn.jsdelivr.net/npm/p5.glitch@latest/p5.glitch.js"></script>
```

### Example Library: Using p5.touchgui

https://github.com/L05/p5.touchgui/ is a library that *overrides* DOM manipulation for p5 specific elements. 

```html
<script src="https://unpkg.com/p5.touchgui@0.5.2/lib/p5.touchgui.js"></script>
```

## Extra Review Materials

### External Resources

- Allison Parrish, [Working with Video](https://creative-coding.decontextualize.com/video/)
- Coding Train `ml5` Playlist [Introducing ml5 using FaceMesh](https://thecodingtrain.com/tracks/ml5js-beginners-guide/ml5/0-introduction/patt-vira)
- Coding Train [Live Video and `createCapture()`](https://thecodingtrain.com/tracks/pixels/pixels/createCapture) Playlist