<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~ README.md of CSS-Advanced for Adv-CSS.bauska.org ~~~~~~~~~~~~~~~~~~~~~-->
<h1>CSS-Advanced</h1>
<p>Folling is left frozen column</p>

Table of Contents
What is Advanced CSS?
Why is Advanced CSS Important?
CSS Pseudo classes
CSS Pseudo elements
CSS Z-Index
What is CSS User Interface?
CSS Blend modes
CSS Transitions and animations
Browser Compatibility of Advanced CSS
Advanced CSS Best practices

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p><a href="https://www.browserstack.com/guide/advanced-css-tutorial">from Browserstack's Advanced CSS Tutorial</a>.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>Tips, tricks, techniques used in advanced CSS methodologies.</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Advanced CSS is the backbone of modern web design, enabling developers to go beyond basic styling and create dynamic, responsive, and visually appealing websites. It involves powerful techniques such as pseudo-classes, transitions, blend modes, and animations — all aimed at improving user experience and performance.</p>
<h2>Overview</h2>
<ul>
  <li>1. What is Advanced CSS in Web Development?
    <ul>
      <li><p>Advanced CSS refers to complex styling techniques that extend beyond simple properties like colors, 
      fonts, and margins.</p></li>
      <li><p>It includes features like pseudo-classes, pseudo-elements, transitions, animations, and responsive layouts.</p></li>
      <li>These capabilities help developers design engaging, scalable, and future-ready interfaces.</p></li>
	</ul>
  </li>
  <li>2. Why is Advanced CSS Important for Modern Websites?
    <ul>
      <li><p><b><i>Enhanced Interactivity</i></b>: Enables hover effects, focus states, and transitions for smoother user experiences.</p></li>
	  <li><p><b><i>Improved Layouts</i></b>: Tools like Flexbox and Grid reduce reliance on JavaScript for responsive designs.</p></li>
      <li><p><b><i>Better Performance</i></b>: Cleaner, modular code with reduced duplication improves maintainability.</p></li>
      <li><p><b><i>Future-Proof Design</i></b>: Ensures compatibility with evolving browser capabilities and design standards.</p></li>
	</ul>
  </li>
  <li>3. How to Use Advanced CSS Techniques Effectively?
    <ul>
      <li><p><b><i>Pseudo-Classes</i></b>: Style elements in different states (:hover, :active, :focus, :first-child, :nth-child).</p></li>
      <li><p><b><i>Pseudo-Elements</i></b>: Target specific parts of an element (::before, ::after, ::first-letter) for refined design control.</p></li>
      <li><p><b><i>Transitions & Animations</i></b>: Add motion and interactivity to elements for a more engaging UI.</p></li>
	  <li><p><b><i>Blend Modes & Z-Index</i></b>: Create layered effects and manage element stacking for complex visual designs.</p></li>
	</ul>
  </li>
  <li>4. Key Best Practices for Writing Advanced CSS
    <ul>
      <li><p>Use <b><i>modular and reusable classes</i></b> to keep code maintainable.</p></li>
      <li><p>Always <b><i>test browser compatibility</i></b> for advanced features.</p></li>
      <li><p>Leverage <b><i>CSS variables</i></b> for consistent styling and easier updates.</p></li>
      <li><p>Combine advanced CSS with responsive design principles for seamless performance across devices.</p></li>
	</ul>
  </li>
</ul>

<p>This article explains what advanced CSS is, why it’s essential, how to implement its key techniques, and the best 
practices to follow for scalable, modern web design.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch1">What is Advanced CSS?</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>As the name suggests, <b>advanced CSS</b> is a set of styling techniques that go beyond a website’s basic styling capabilities 
such as fonts, colors, margins, and more.</p>

<p>Whereas <b>advanced CSS</b> contains complex and advanced style design features such as pseudo-classes, animations, transitions, 
and more that enhance aesthetics and functionality, ultimately improving the user experience.</p>

<p>Incorporating advanced CSS into your projects enhances a website’s visuals, creates a scalable codebase, and improves its responsiveness.</p>

<cite>Also Read: <a href="https://www.browserstack.com/guide/elements-of-modern-web-design">10 Core Elements of Modern Web Design</a></cite>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch2">Why is Advanced CSS Important?</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>As the internet evolves, expectations for aesthetics, performance, and responsiveness also increase. Therefore, advanced CSS is important to tackle such a situation and create a future-proof website.</p>

<h3 id="ch1-1">Here are a few reasons why Advanced CSS is essential:</h3>
<ul>
  <li>Techniques such as Flexbox and CSS Grid reduce the dependency upon JavaScript and frameworks for creating responsive layouts.</li>
  <li>It leverages animations and transitions to create a smooth user experience that increases the satisfaction rate of users who visit your websites.</li>
  <li>Advanced CSS techniques allow for a cleaner codebase, avoid duplication, and are scalable.</li>
  <li>Advanced CSS techniques also allow you to future-proof your projects by ensuring modern web designs that are adaptable and compatible with evolving browser standards.</li>
</ul>
<h3>CSS Pseudo Classes#</h3>
<p>CSS Pseudo Classes are a set of keywords that are used along <a href="https://www.browserstack.com/guide/css-selectors-in-selenium">CSS selectors</a> to style a dynamic state of an element.</p>

<p>For example, you want to design a button. However, you want to ensure a slightly different design when the mouse hovers over the button and when it is clicked. In situations where you want to style the dynamic conditions of an element, <b>pseudo-classes</b> are used.</p>

<p>A pseudo-class consists of a <b>colon (:)</b> followed by the <b>pseudo-class name</b> (e.g., hover) and is attached to <b>anchor element</b> (e.g., button in case button: hover).</p>

<h4>Hover pseudo class</h4>
<p>The hover pseudo-class applies styles when the mouse hovers over an element.</p>

<h4>Syntax:</h4>

```
selector:hover {
  /* styles */
}
```

<h4>Example:</h4>

<p>Consider an example where a button is created, and the pseudo-class is used to change its appearance when hovered.</p>

<h4>Index.html:</h4>

```
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <button class="button">Hover me</button>
  </body>
</html>
```

<h4>Style.css:</h4>

```
.button {
  background-color: blue;
  border-radius: 8px;
  border-style: none;
  color: white;
  cursor: pointer;
  font-family: sans-serif;
  font-size: 14px;
  padding: 10px 16px;
  text-align: center;
}
```

<h4>hover pseudo class</h4>

```
.button:hover{
  background-color: red;
}
```

<h4>hover pseudo class 2</h4>

<h3>Active pseudo class</h3>
The active pseudo-class is applied to an element when the user clicks (presses down) an element that has yet to be released.

<h4>Syntax:</h4>

```
selector:active {
  /* styles */
}
```

<h4>Example:</h4>

To demonstrate, create a placeholder(input box), which changes its appearance when the user clicks on it.

Note that the effect restores to the original upon releasing the mouse button.

```
input {
  padding: 10px;
  font-size: 16px;
  border: 2px solid #ccc;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}
/* Styling the placeholder */
input::placeholder {
  color: gray;
}
```
<h4>active pseudo class</h4>
```
input:active::placeholder {
  color: red;
}
input:active {
  border-color: blue;
  background-color: #f0f8ff;
  outline: none;
}
```
active pseudo class 2

First child and last child
The first-child and last-child pseudo-classes are used to style the first and last-child elements within a parent container, respectively.

Syntax:
```
selector:first-child {
  /* styles */
}
selector:last-child {
  /* styles */
}
```
Example:

To demonstrate, consider a scenario with multiple paragraph elements within a container, where only the first and last paragraphs need to be styled, leaving the rest unchanged.

```
<div>
  <p>This is the first paragraph.</p>
  <p>This is the second paragraph.</p>
  <p>This is the last paragraph.</p>
</div>
<style>
  p:first-child {
    color: red;
  }
  p:last-child {
    color: blue;
  }
</style>

first child and last child output image

<h3>Nth child()</h3>
The nth-child() pseudo-class lets you select elements for styling based on their position with the parent element.

<h4>Syntax:</h4>

```
selector:nth-child(n) {
  /* styles */
}
```
Here, “n” takes values of the position of the children to select. It can take numeric values as well as a keyword such as odd and even.

<h4>Example:</h4>

To demonstrate, consider a scenario with multiple paragraph elements within a container, where only the third paragraph needs to be styled while the others remain unchanged.

```
<div>
  <p>This is the first paragraph.</p>
  <p>This is the middle paragraph.</p>
  <p>This is the last paragraph.</p>
</div>
<style>
  p:nth-child(3){
    color: red;
  }
</style>
```

<h4>Focus</h4>
The focus pseudo-class lets you style elements when an element is focused through keyboard navigation or mouse clicks.

Unlike the active pseudo-class, the mouse can be released and not pressed all the time. It is a helpful technique while designing form elements such as <input>, <textarea>, and <select>.

<h4>Syntax:</h4>

```
selector:focus {
  /* styles */
}
```

<h4>Example:</h4>

```
input {
  padding: 10px;
  font-size: 16px;
  border: 2px solid #ccc;
  border-radius: 5px;
}
/* Styling the placeholder */
input::placeholder {
  color: gray;
}
```

<h4>focus pseudo class e1730537153299</h4>

```
input:focus::placeholder {
  color: rgb(60, 0, 255);
}
input:focus {
  border-color: rgb(255, 42, 0);
  background-color: #f4ae95;
  outline: none;
}
```

<h4>focus pseudo class 2</h4>

<h3>Target</h3>
The target pseudo-class allows you to style an element when the URL contains a hash (#) followed by the id of that element to be styled. This is often combined with anchor links to show or hide content dynamically.

<h4>Syntax:</h4>

```
selector:target {
  /* styles */
}
```

Also Read: Top Responsive CSS Frameworks

<h3>CSS Pseudo-Elements#</h3>

Pseudo-elements in CSS are also special keywords in CSS tusing which you can style specific parts of an element without changing the underlying HTML structure. Unlike Pseudo classes that style different states or conditions of an element, the CSS pseudo-elements style part of an element and can also insert, remove, and modify an element without changing the HTML structure.

CSS pseudo-element consists of a double colon (::) followed by the pseudo-element keyword(e.g., h1::before).

<h4>First letter pseudo element</h4>

The first-letter pseudo-element styles only the first letter of block-level text elements, such as paragraphs, headings, and other text-displaying content. It can’t be used for inline elements as it leverages elements’ ability to break lines for larger text formatting.

<h4>Syntax:</h4>

```
selector::first-letter {
  /* styles */
}
```

<h4>Example:</h4>

```
p::first-letter {
  font-size: 3em;  /* Make the first letter 3 times larger */
  color: red;      /* Change its color to red */
  font-weight: bold; /* Make it bold */
  float: left;     /* Float the letter to the left */
  margin-right: 5px; /* Add space between the letter and the rest of the text */
}
```

<h4>first letter pseudo element</h4>

<h4>before Pseudo element</h4>

The before pseudo-element is used to insert content before the content of any element without altering its HTML structure.

<h4>Syntax:</h4>

```
selector::before {
  /* styles or content */
}
```

<h4>Example:</h4>

<h4>Index.html:</h4>

```
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Pseudo-Elements </title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Pseudo Elements: BrowserStack</h1>
</body>
</html>
```

<h4>Style.css:</h4>

```
h1::before {
  content: "★\A ";
  color: gold;
  font-size: 1.5em;
  white-space: pre; }
```

<h4>before Pseudo element</h4>

Also Read: How to position text over image using CSS

<h3 id="CSS-Z-Index">CSS Z-Index</h3>
The Z-Index in CSS is a property used to control how the elements are stacked on a webpage. In simpler words, it ensures how elements are placed on top of one another.

To place any aspect on top of another, the element must have a z-index value higher than that element to be placed below.

It is used to manage overlapping elements, such as in designing a dropdown, a tooltip, floating elements, dialogue boxes, and more.

<h4>Syntax:</h4>

```
selector {
  z-index: value;
}
```

Here value can take inputs such as a positive number, a negative number, and an auto. Auto is the default value and follows the natural order of elements. Element with a higher value of Z-index will be at the top.

<h4>Example:</h4>

In this example, let’s create four boxes and manage their stacking with the help of z-index.

<h4>Index.html:</h4>

```
<!DOCTYPE html>
<html lang="en">
<head>
  <title>z-index Example</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="box box1"></div>
  <div class="box box2"></div>
  <div class="box box3"></div>
  <div class="box box4"></div>
</body>
</html>
```

<h4>Style.css:</h4>

```
.box {
  width: 150px;
  height: 150px;
  position: absolute;
  opacity: 0.9;
}
.box1 {
  background-color: red;
  top: 50px;
  left: 50px;
  z-index: 4; /* Highest stacking order */
}
.box2 {
  background-color: blue;
  top: 100px;
  left: 100px;
  z-index: 3; /* Higher stacking order */
}
.box3 {
  background-color: green;
  top: 150px;
  left: 150px;
  z-index: 2; /* High stacking order */
}
.box4 {
  background-color: black;
  top: 200px;
  left: 200px;
  z-index: 1; /* Lowest stacking order */
}
```

<h4>z index</h4>

However, the natural order of elements is as:

<h4>Z index natural</h4>

<h3 id="What-is-CSS-UI">What is CSS User Interface?</h3>
CSS User Interface contains several properties that allow control of the behavior and appearance of user interface elements on a webpage. CSS provides many user interface features, such as resizing elements, outlines, box-sizing, and more.

Resize and Outline-offset are the most common and important CSS UI features.

Learn More: How to Create Browser Specific CSS Code

<h4>Syntax for CSS UI resizing</h4>

It allows the element to be resized by the user and is most commonly found in text areas and div.

```
selector {
  resize: value;
}

```

<h4>Value: none, both, horizontal, or vertical.</h4>

<h4>Syntax for CSS UI outline</h4>

It is used to draw a line outside the element’s border for better focus.

```
selector {
  outline: value;
}
```

<h4>Value: outline-width, outline-style, or outline-color.</h4>

<h3 id="CSS-Blend-Mode">CSS Blend Modes#</h3>
This feature of CSS is inspired by photo editing software, where images are often blended to create a good composition and make it visually appealing.

CSS offers two blend modes to directly blend colours within the webpage.

<h4>background-blend-mode</h4>
It controls how multiple background layers blend.

```
selector {
  mix-blend-mode: value;
}
```

Here value takes blending operations such as multiply, screen, overlay, darken, lighten, color-dodge, color-burn, difference, and more.

<h4>Mix-blend-mode</h4>
It controls how the content of an element blends with the content of its parent or sibling elements(or background).

```
selector {
  background-blend-mode: value;
}
```

Here value takes the blending mode used between background layers such as overlay, screen, multiply, and more.

<h4>CSS Transitions and Animations#</h4>
CSS Transitions provide a change from one property to another over a specific duration rather than instantly, whereas CSS Animations set keyframes to animate transitions.

Both are very powerful CSS features that create appealing visuals for a website.

<h4>CSS Transitions Syntax</h4>

<h4>transition: property duration timing-function delay;</h4>

property: The CSS property you want to animate (e.g., background-color, width, height).
duration: duration of transition (e.g., 1s for one second).
timing-function: Specifies the speed curve of the transition (e.g., ease, linear, ease-in-out).
delay: Specifies the delay before the transition starts.

Example: In this example, a blue box turns into green and scales up (size increases) when it is hovered, however, the transition property makes this change occur over 0.5s with an ease timing function.

<h4>Index.html:</h4>

```
<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Transition</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="box"><h2>Hover Me</h2></div>
</body>
</html>
```

<h4>Style.css:</h4>

```
.box {
  width: 100px;
  height: 100px;
  background-color: blue;
  transition: background-color 0.3s ease, transform 0.3s ease;
}
.box:hover {
  background-color: green;
  transform: scale(1.2);
}
```

<h4>translate GIF</h4>

<h4>CSS Animations Syntax</h4>

<h4>1. @keyframes</h4>

```
@keyframes animation-name {
  0% { /* Starting state */ }
  50% { /* Midpoint state */ }
  100% { /* Ending state */ }
}
```

</h4>h4>2. Animation Properties</h4>

```
animation: animation-name duration timing-function delay iteration-count direction;
```

<ul>
  <li><b>animation-name</b>: Name of the animation defined by @keyframes.</li>
  <li><b>duration</b>: duration for the animation(e.g., 2s).</li>
  <li><b>timing-function</b>: speed of the animation (ease, linear, ease-in, etc.).</li>
  <li><b>delay</b>: Time before the animation starts (e.g., 1s).</li>
  <li><b>iteration-count</b>: Number of times the animation should run (infinite for continuous looping).</li>
  <li><b>direction</b>: The direction of the animation (normal, reverse, alternate, etc.).</li>
</ul>

<h4>Example:</h4>

A simple example of a box moving horizontally and changing color.

<h4>Index.html:</h4>

```
<!DOCTYPE html>
<html lang="en">
<head>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="box"></div>
</body>
</html>
```

<h4>Style.css:</h4>

```
.box {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation: moveAndChange 3s ease-in-out infinite alternate;
}
@keyframes moveAndChange {
  0% {
    left: 0;
    background-color: red;
  }
  50% {
    left: 150px;
    background-color: green;
  }
  100% {
    left: 300px;
    background-color: blue;
  }
}
```

The animation runs for <b>3s</b>, with an <b>ease-in-out</b> timing with <b>alternate</b> back and forth and <b>infinite</b> running.

<ul>
  <li><b>At 0%</b>, the box has a red background at the leftmost part.</li>
  <li><b>At 50%</b>, the box moves 150px right and turns green.</li>
  <li><b>At 100%</b>, the box moves 300px right and turns blue.</li>
</ul>

After that, it repeats back and forth motion infinitely.

Browser Compatibility of Advanced CSS#
If you’re using these Advanced CSS techniques in your project, you must understand that although the newer versions of browsers show robust support for these methods and practices, the older versions of popular browsers mostly don’t, which leads to inconsistent behaviour across different platforms.

<a href="https://www.browserstack.com/guide/browser-compatibility-with-css-gradients">Browser Compatibility</a> is a crucial factor in determining the success of your website. Therefore, you must perform ample testing on your project before rolling it out to the world to ensure <a href="https://www.browserstack.com/guide/how-to-ensure-test-coverage">maximum test coverage</a>.

However, setting up a lab of physical devices can be both costly and bothersome.

Image of: BrowserStack Responsive Testing Banner

A great solution is to set up a real device cloud. BrowserStack gives you access to 3500+ browsers and actual device combinations (mobile and desktop), providing wide coverage for Cross Browser & Platform Testing.

You can also save time by leveraging parallel testing on BrowserStack, running tests across multiple browser-device combinations simultaneously. This helps developers and testers create applications that deliver a seamless user experience, enhancing user retention and satisfaction.

Image of: Pseudo class support on different browser versions 1

<a href="https://www.browserstack.com/guide/advanced-css-tutorial#">Talk to an Expert</a>

Here’s an example of pseudo-class support on different browser versions from older to the latest on 
<a href="https://caniuse.com/css-matches-pseudo">Can I Use</a>.

<h3>Advanced CSS Best Practices#</h3>
The primary concern behind knowing the best practices is to create an efficient code base that is scalable, maintainable, easy to update, and properly structured.

Here are some of the best Advanced CSS practices to maintain healthy and efficient coding:

1. Use CSS variables for reusable values such as fonts, colors, and more.

```
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --font-size-base: 16px;
}
body {
  background-color: var(--primary-color);
  font-size: var(--font-size-base);
}
button {
  background-color: var(--secondary-color);
}
```

2. To create layouts, prefer Flexbox and CSS grid as they align with the website’s responsiveness.

3. As the number of mobile users is increasing rapidly, you must consider the mobile-first approach. According to this, you first design the website for mobile and then gradually expand to larger screens. This also creates good responsiveness on your website.
4. Use animations and transitions appropriately and wisely. Although they enhance user experience, using them extensively slows down your website.
5. Use CSS Shorthand to make your script more concise, and readable, and reduce the amount of code.

```
margin-top: 10px;
margin-right: 20px;
margin-bottom: 15px;
margin-left: 30px;

/* Use this */
margin: 10px 20px 15px 30px;
```

Advanced CSS is a set of techniques that is built upon the foundation of basic CSS. It contains advanced techniques such as pseudo-classes, animations, and transitions that enhance both aesthetics and functionality, ultimately improving the user experience.

Older browser versions don’t support many advanced CSS techniques. Therefore, to ensure maximum coverage, you must perform Cross-Browser Testing before launching your application for real-world users.

<a href="https://www.browserstack.com/real-device-cloud">Test on Real Devices</a>

<h4>Tags:</h4>
<ul class="horizontal-list">
  <li><a href="https://www.browserstack.com/guide/tag/ui-testing">UI Testing</a></li>
  <li><a href="https://www.browserstack.com/guide/tag/visual-testing">Visual Testing</a></li>
  <li><a href="https://www.browserstack.com/guide/tag/website-testing">Website Testing</a></li>
</ul>

```
ul.horizontal-list {
  display: flex;         /* Automatically aligns items in a row */
  list-style-type: none; 
  gap: 20px;             /* Easily sets the space between items */
}
```
