# Week 01

## Agenda

1. Syllabus, Expectations and Class Manifesto
2. Introductions
3. Introduction Survey
4. Break
5. Intro to Coding
6. Tutorial: Drawing with p5.js
7. Demos, Videos, and Useful Links

## Syllabus

- Read through the [syllabus](https://github.com/samheckle/hunter-creative-code-fa-26/blob/main/readme.md): https://github.com/samheckle/hunter-creative-code-fa-26/blob/main/readme.md (and bookmark it! this is also where class notes will live!)
- If I am ever going too fast through _any_ material, please interrupt me!
- Questions? Comments? Needs? Etc? Send an email. I value open communication more than anything else. If you miss class, expect to be late, or are struggling with an assignment, please let me know.
### Expectations and Class Manifesto

1. Be curious!
   - what questions are you asking?
	   - Good questions to ask ***in class***:
		   - Will you repeat the last thing you said?
		   - Could you give another example?
		   - Could you go through that again, slower?
		   - Will you explain “blah” in a different way?
		   - Can you explain that word “blah” you said?
		   - Can you please speak a little slower?
   - what do you not know?
   - how can you find those answers?
     - Reach out to your buddy
     - Talk to [Hunter CS Club](https://huntercsclub.com/)
     - Post your question in the [p5.js Discourse Forum](https://discourse.processing.org/c/p5js/10) or in [p5js Discord](https://discord.gg/kFMvWNQMeu)
1. Practice!
   - learning to code takes time!
   - you _will_ have to do a lot of work outside of class to understand what is going on in the context of your own projects
3. Low Stress **NOT** Low Effort
   - did you learn something new? write it in your documentation!
   - did you struggle? write it in your documentation!
   - did you accomplish what you wanted? write it in your documentation!
   - if you made a solid attempt and wrote documentation (via a discussion post) you get full credit!

### Class Format

Broadly – this is similar to a math class, sprinkled with media theory and artmaking.

You will be taught in class:

- syntax of how the coding language works
- application of how to use the coding language in your artistic practices

Outside of class:

- practice the syntax
- contextualize the content in your own projects

A typical week structure might look like:

1. Review previous week’s assignment and questions
2. Review lecture & discussion
3. Practice new content in class
   - You should be following along the demos!
1. Apply new content in upcoming assignment

### A Note on AI

We already discussed AI policy in the syllabus, but it is important to note here that by learning to code we are becoming more computer literate. We are gaining a deeper understanding of the inner workings of our machines that are so intertwined with our lives. Dedicating the time now to deepen that understanding will broaden your capabilities for your work going forward. It is ***strongly encouraged to limit your AI use*** to tutoring and understanding for the first half of the course as we build out our foundations of coding.

As mentioned previously, it is suggested to include in your prompts:
- "Do not give me the answer, but help me work out how to read through this error message"
- "Walk me through this code snippet line by line. I don't understand why line 24 exists"
These are *very* specific and targeted prompts, as if you were talking to a tutor. Your skills will not deepen if you copy-and-paste every assignment.
## Introductions

### Me: sam heckle (they/she)

- software engineer to creative technologist pipeline
- things you can ask me about: creative coding, software engineering, net art, permacomputing, networks, media theory, portfolio review, resume review, games, keyboards, galleries. ***please ask me about these things in [office hours](https://calendly.com/samanthaheckle/30min)***
<img src="https://github.com/samheckle/images/blob/main/intro.png?raw=true" style="width=600px">


### Introduction survey

Please fill out this [survey](https://forms.cloud.microsoft/r/aWPXrkseXm).

## Introduction to Code

### Tutorial: Learning about p5 Editor

Make an account: <https://editor.p5js.org/>

#### Looking at the p5 Editor

| Click the Gear Icon in the Upper left. |                                                                                                                |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| These are my preferred settings.       | ![p5 settings](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/settings.png?raw=true) |
### Writing and Running Code

![p5.editor](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/p5_editor.png?raw=true)

### General Flow

| How to submit homework                                 |                                                                                                     |
| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| 1. Rename sketch to enable saving                      | ![name](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/1.png?raw=true)    |
| 2. Save your sketch (you can also press ⌘+S or Ctrl+S) | ![save](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/2.png?raw=true)    |
| 3. Finish your assignment...                           |                                                                                                     |
| 4. Tidy your code                                      | ![save](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/tidy.png?raw=true) |
| 5. Retrieve the URL and submit.                        | ![save](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/url.png?raw=true)  |
## Definitions: Coding Glossary vs. p5 Glossary

#### Coding Glossary

These terms that can be used _universally_ when talking about code, so if you know others who are familiar with coding likely they will know what you mean when using these terms. There will always be terms that will be distinguished between general terms vs. p5 specific terms.

| coding glossary           |                                                                                                                                                                          |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| algorithm                 | series of steps to execute to solve a problem                                                                                                                            |
| syntax                    | grammars or punctuation of the language you code in                                                                                                                      |
| JavaScript                | a programming language, often used for the web. Not to be confused with Java, a different programming language.                                                          |
| p5.js                     | a JavaScript library, which follows most JavaScript rules, but also defines its own.                                                                                     |
| documentation / reference | a dictionary for syntax of a particular coding language. For us, this means we will be using https://p5js.org/ (another bookmark!). This is the "textbook" of the class. |
| comment                   | a note embedded inside of code                                                                                                                                           |
| function                  | an instruction or command, may or may not have **_parameters_**, also known as _method_                                                                                  |
| parameter                 | value that is passed into the `()` of the function, also known as _arguments_                                                                                            |
#### Comments

A comment is a way in javascript to write notes and organize your code.

```js
// this is a comment
// we write comments in our code to explain what is going on and to organize ourselves
// you don't need to copy the comments i write, you are welcome to take your own notes
```

It is helpful to write comments not only to explain what a particular piece of code does, but especially so if you come back to an assignment much later on. As we will be submitting your demos at the end of class, it is great to write comments on parts you found easy or difficult.

#### Function

```js
// the syntax of a function is the name followed by parenthesis
functionName();
```

#### Parameter

```js
// parameters go inside the parenthesis
functionName(parameterValue);
```

some p5 examples of functions with and without parameters

```js
// without parameters
beginShape();

// with parameters
fill(255);
background(255);

// with multiple parameters, separated by a ,
createCanvas(400, 400)
```

#### `p5.js` Glossary

The p5 glossary are terms that are specific to the `p5.js` library and our class.

| `p5.js` Glossary |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| sketch           | the name of the programs you are making for this class.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| `setup()`        | a function that happens before the animation loop and _executes one time_. once it completes, it moves to the next line in the code.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| `draw()`         | is the animation loop, executes with framerate                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| canvas           | the area on the screen where the code is executed, similar to an artboard. uses the cartesian coordinate system (x, y). <br>![coordinates](https://github.com/samheckle/code-toolkit-fa-25/blob/main/images/week_01/coordinates.png?raw=true) <br>Important to note here is the blue line represents the x-axis, increasing from left to right. The red line represents the y-axis, increasing from top to bottom. `(0, 0)` starts from the top left corner and increases until the `width` and `height` have been reached. The width and height are determined by the parameters passed in to the `createCanvas()` function located in setup. |

### `setup()` and `draw()`

These are two functions that are created for us in every p5 sketch. They use `{}`, and *all of our code must be written inside them* (for now). 

For example:

```js
function setup(){
	// i can start writing code below this line with the open {

	// i stop writing code before this line with the close }
}
```

### Walking through using a `p5.js` function

Let's draw a rectangle! To start, we can open up the reference (https://p5js.org/reference/) to see what we can do, and navigate to [Shape](https://p5js.org/reference/#Shape). 

From here, we can see how to make a rectangle: https://p5js.org/reference/p5/rect/

The general flow of each reference page is:
1. Title of the page with the generic line of code (ex: `rect()`)
2. Description of what that does 
3. Example of how it works with an embedded editor
4. Syntax
5. Parameters
6. Related Reference

For me, I usually read the description and skip directly to the syntax section to understand the code better.

```js
rect(x, y, w, [h], [tl], [tr], [br], [bl])
```

We can see the detail of each of the parameters (so `x`, `y`, `w`, `[h]`, `[tl]` etc.) in the parameter description beneath it. Anything that is indicated by `[]` means it is an *optional parameter*, so we don't need to include it. But, ***order matters*** in code. 

When we write our sketches, we write it in order from top to bottom, left to right. Each line is numbered, and every character in the line is important for the computer to understand what you are trying to communicate. `createCanvas()` happens before `background()` because we need to have a place to put the background before we give it a color.

For parameters in a function, we need to match how the computer understands which order the `x`, `y`, `w`, and `h` values go. I always find myself going back to the reference. **You are not expected to memorize syntax**, but you are expected to remember the patterns and rules of how the syntax operates.

So, I might not remember the order in which a rectangle is drawn, but I know that it requires 3 parameters, the parameters go inside `()` and the function name is `rect()`. I might not remember which order the `x`, `y`, `w` values are, but I can always look at the reference. Something I find useful is to copy the syntax into a comment:

```js
// rect(x, y, w, [h], [tl], [tr], [br], [bl])
rect(100, 150, 100, 300)
```

Based on the *left to right order*, the computer translates where the rectangle should go `(100, 150)` and how large it should be `100x300px`

```
x = Number: x-coordinate of the rectangle    = 100
y = Number: y-coordinate of the rectangle    = 150
w = Number: width of the rectangle           = 100
h = Number: height of the rectangle          = 300
```
## References and Useful Review

### References
- The Critical Engineers Manifesto: https://criticalengineering.org/
### Extra Review Materials
- [Learning to Learn (to program)](https://teachinglondoncomputing.org/learning-to-learn-to-program/)
- [So you want to be a wizard](https://wizardzines.com/zines/wizard/) (zine)
- History of `p5.js`: https://www.youtube.com/watch?v=FdsWWjqoPKU
- More explainers on Intro to `p5.js`:
	- [How to use the web editor (1.2)](https://youtu.be/MXs1cOlidWs?si=t58V0PMAPYaIr9Es)
	- [Shapes & Drawing 1.3](https://youtu.be/c3TeLi6Ns1E)
	- [Color 1.4](https://youtu.be/riiJTF5-N7c)
	- [Errors 1.5](https://youtu.be/LuGsp5KeJMM)
	- [Comments 1.6](https://youtu.be/xJcrPJuem5Q)
