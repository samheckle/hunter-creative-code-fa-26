## Agenda

1. Housekeeping
2. Project #4 Presentations
3. Tutorial: The Web
4. Extra Review Materials

## Housekeeping

1. Attendance 
2. Schedule for the rest of the semester

## Project 4 Presentations

Every group member should pull up their project on a computer. We will go around the room and play each project and talk about some observations. Then we will get to presentations. Each group will have maximum 10 minutes to present, including critique. 

## The DOM

| coding glossary |                                                                                                                                           |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| HTML/CSS        | markup languages that determine the structure + style of web pages, inside `index.html` and `style.css`                                   |
| HTML            | Hyper-Text Markup Language is a way of "tagging" text to define the structure of a web page                                               |
| element / tag   | in HTML, a specific item on the page, eg. `<p>`, `<a>`, `<div>`                                                                           |
| flow layout     | how HTML is displayed in the browser. it reads from the top to the bottom according to how big the page is and how much content you have. |
| attribute       | extra information for an HTML tag that always goes in the opening tag of an element. it follows the syntax `attributeName=""`             |
| DOM             | the Document Object Model, which allows us to manipulate HTML/CSS with JavaScript.                                                        |

### HTML

Hyper-text markup language (HTML) defines the structure of a webpage using a series of tags, enclosed in `< >`.

```html
<!-- this is a comment -->
<!-- this is an opening tag -->
<html>
	<!-- this is a closing tag -->
</html>
```

Looking at the default `.html` file inside our p5 editor:

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<script src="https://cdn.jsdelivr.net/npm/p5@1.11.10/lib/p5.js"></script>
		<script src="https://cdn.jsdelivr.net/npm/p5@1.11.10/lib/addons/p5.sound.min.js"></script>
		<link rel="stylesheet" type="text/css" href="style.css" />
		<meta charset="utf-8" />
	</head>
	<body>
		<main> </main>
		<script src="sketch.js"></script>
	</body>
</html>
```

`<html>` has two "child" elements, meaning tags that are nested between the opening and closing tags.

- `<head>` gives us extra data about the webpage, but it isn't seen inside the page
- `<body>` is the actual content of the page

Other html tags (not a definitive list):

- `<p>` - paragraphs
- `<em>` - emphasis / italics
- `<strong>` - bold
- `<img>` - images, use `src` attribute to determine paths to files
- `<a>` - links, uses `href` attribute to go to another file or site

Take a look at the [full list of html tags on the docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements).

### CSS

Cascading style sheets determine the style, or what the web page looks like. This is a series of rules that look very similar to objects with properties. They are given via a selector.

```css
/* this is a comment in css */

p {
	/* selector, or which tag/element we want to apply the style to*/
	color: blue; /* rule in key:value pair */
}
```

We can see a [full list of css properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties) in the documentation.

Looking at the default `.css` in the p5.editor:

```css
html,
body {
	margin: 0;
	padding: 0;
}
canvas {
	display: block;
}
```

### DOM

The Document Object Model is the way that Javascript is able to perceive and reference HTML code to make changes to it.

![dom](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/example-dom-tree.svg)

This enables us to programatically add items to the DOM using p5.js: https://p5js.org/reference/#DOM

## Extra Review Materials

- Allison Parrish [Browser Controls](https://creative-coding.decontextualize.com/browser-controls/)
- Coding Train [HTML/CSS/DOM Playlist](https://www.youtube.com/watch?v=URSH0QpxKo8&list=PLRqwX-V7Uu6bI1SlcCRfLH79HZrFAtBvX) (videos 8.1-8.16)