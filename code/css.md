# 💻 CSS

#### Overview

CSS (Cascading Style Sheets) is a styling language that describes how elements should be rendered in the browser. CSS modifies the presentation of the HTML code. CSS is the dress up of coding languages.

#### Vocabulary

- CSS
- separation of concerns
- selector
- declaration
- key:value pair
- property
- splat
- pseudo selectors

#### Additional Resources

- [W3Schools CSS](https://www.w3schools.com/w3css/defaulT.asp)
- [CSS Properties](https://www.w3schools.com/cssref/index.php)
- [Google Fonts](https://fonts.google.com/)
- [CSS Tricks Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Flexbox Froggy](http://flexboxfroggy.com/)
- [Flexbox Defense](http://www.flexboxdefense.com/)
- [CSS Animation for Beginners](https://thoughtbot.com/blog/css-animation-for-beginners)
- [Color Wheel](https://www.canva.com/colors/color-wheel/)

#### Process

- Create a new file in your `jumpstart` folder called `treasurehunt.css`

#### Troubleshooting Tips

- Is the stylesheet connected to the HTML page?
- Did you save your file?
- Did you refresh your browser?

---

### CSS Fundamentals

CSS stands for Cascading Style Sheets. **CSS** is a stylesheet language used to modify the presentation and behavior of HTML tags. CSS doesn’t do much without HTML for it to act on.

CSS styling can be written once, and used multiple times in your HTML code. Creating a styling sheet helps us achieve the coding philosophy of **separation of concerns** which divides responsibility between different areas of your code into different files. It also allows us to make the code DRY, which stand for Don't Repeat Yourself.

Styling in CSS can be more difficult that expected. It often comes down to a lot of trial and error, so don’t be discouraged. There are lots of online resources to help.

The building blocks of CSS are selectors and declarations. A CSS **selector** targets an HTML tag allowing stylings to be applied. There are three ways to create selectors. We can target the name of an HTML tag, target an id or target a class. The selector is followed by a set of curly braces. Inside the curly braces are the CSS declarations. A CSS **declaration** is a key:value set with a CSS property and the following modifier value.

Selectors that reference an HTML tag will apply styling to every instance of that tag. To target a tag's id use the pound sign `#` in front of the name of the id. To target a class use a period `.` in front of the name of the class.

The declarations are sets of **key:value** pairs. The key is a CSS property. There are many, many CSS **properties** which provide the browser with information on how to display the style. The value is what the property will be changed into. For example, to change the font color of the `h1` tag in HTML we would apply a property of `color` and the value of the color we want it to become.

A selector can have as many properties as needed. Each property is separated from the others with a semicolon.

```css
/* tag selector with a property key:value pair */
h1 {
  color: blue;
}

/* id selector with two CSS properties */
#the-id-name-here {
  padding: 20px;
  font-size: 30px;
}

/* class selector */
.the-class-name-here {
  background-color: pink;
}
```

### Creating CSS

Inside the project folder create a new file called `treasurehunt.css`. Using the correct file extension will enable your text editor to give you hints and suggestions to make your coding easier and faster. It also can be a fun way to explore what style properties are available.

The stylesheet file will become a dependency of the HTML file. So it will need to be linked into the `head` tag.

```html
<link rel="stylesheet" href="treasurehunt.css" />
```

### CSS Tips and Tricks

Colors in CSS can be referenced in two different ways. CSS recognizes a large number of color names. We can use color names such as black, blue, and purple as well as aquamarine, coral, honeydew, tomato, and many others. If we want a color that is more specific we can use a hex code. A **hex code** is a hexadecimal format representing how much red, green, and blue exist in a color. The format looks like this: `#RRGGBB`. The hex code can be passed as a value to the color property.

```css
/* color property with a color name value */
p {
  color: cornflowerblue;
}

/* color property with a color hex code value */
p {
  color: #e1a4b8;
}
```

Particular CSS properties have a shortcut that allows multiple values to be listed together as long as they are in a particular order.

```css
#header-section {
  border-radius: 2px;
  border-style: solid;
  border-color: black;
}
```

Can also be written as:

```css
#header-section {
  border: 2px solid black;
}
```

There is a selector that will apply stylings on every single tag. This is noted by the `*` also known as the **splat**.

```css
* {
  margin: 0;
  padding: 0;
}
```

### Google Fonts

Google fonts are a fun way to modify the page. We can access the [Google font](https://fonts.google.com/) page and select whatever font we like.

Clicking on the `selected family` option at the top of the page will open a sidebar. This will provide two important pieces of information. We can copy the content from the `<link>` tag and paste it into the HTML head tag. This will create a dependency for the information needed to access the particular font. Then we can copy the CSS rules from the sidebar and add to whatever CSS selector we want.

If we want to have the font applied to the entire page we can use the splat selector.

For example:

```css
* {
  font-family: "Lobster", cursive;
  font-family: "Open Sans", sans-serif;
}
```

### Background Image

Backgrounds can be modified a number of ways. Since we want to modify the background of the entire page, the CSS selector is often the HTML `body` tag.

One way is to add a solid color with a color name or hex code. We can also add a color gradient. Gradients have different properties that will change the gradient axis. The gradient takes at least two values of the colors at each end of the gradient.

We can also add an image to the background. The background image often needs additional modification. Like all CSS, this is often a trail and error process.

```css
/* a solid color background */
body {
  background-color: #cccccc;
}

/* a background gradient */
body {
  background-image: linear-gradient(red, yellow);
}

/* a background image */
body {
  background-image: url("img.jpg");
}

/* additional modifications for backgrounds */
body {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

/* Place text in the middle of the image */
.background {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}
```

### Hover Attributes

There is a particular subset of CSS attributes called pseudo selectors. **Pseudo selectors** act on other attributes to make modifications to the styling. A common pseudo selector is a hover attribute that would only show a particular styling when the cursor is over the HTML tag.

Note: this attribute will not behave well on mobile apps as the "cursor" on your phone is your finger or stylus touching the screen rather than a cursor.

```css
/* unvisited link */
a:link {
  color: pink;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  cursor: pointer;
}
```

### Positioning Content

Positioning content on a page is surprisingly challenging. There are a lot of tools that can help make it a little easier. We really like [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/). **Flexbox** is a CSS library that offers a collection of declarations that target parent and child containers. To position something on the page you have to give context. The child container will be nested inside the parent container.

To get a feel for the different ways we can position content, [flexbox froggy](http://flexboxfroggy.com/) is a fun game that will show you the tools.

To center our treasure hunt game board, we can use flexbox. We will have to add a `div` to the HTML to wrap the table. We will target the `div` and give it an id. The id will become the CSS selector.

```html
<div id="gameboard">
  <table>
    ...
  </table>
</div>
```

```css
#gameboard {
  display: flex;
  justify-content: center;
}
```

We can add one more flexbox declaration that will center the text inside each square.

```css
#gameboard {
  display: flex;
  justify-content: center;
  text-align: center;
}
```

### Animation

Animations are a subset of CSS that create movement and action on an HTML tag. To create animation we need to declare the name of the animation and how long the animation should last. Once the animation has a name, we can use a property called `@keyframes`. Inside the keyframe there is a series of frames that range from 0-100%. The change between each of the numbers creates the movement or action. There can be as many frames as needed.

```css
h1 {
  animation-duration: 4s;
  animation-name: heading;
}

@keyframes heading {
  0% {
    transform: scaleX(0.5);
    opacity: 0;
  }
  60% {
    transform: scaleX(1.6);
    opacity: 1;
  }
  100% {
    transform: scaleX(1);
  }
}
```

[CSS animation for beginners](https://thoughtbot.com/blog/css-animation-for-beginners) has a great explanation for each of the animation attributes. There is a list of different ways to use [transform functions](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function).

---

### 💎 Treasure Hunt Challenge

Add a link tag to the head of the HTML page to create a dependency stylesheet.

This is an opportunity for you to explore styling. There are many, many possibilities for creating a look for your game, have fun and be creative!

---

[Back to the top](#-css)

[Back to the main page](../README.md)
