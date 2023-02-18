# 💻 CSS

#### Overview

CSS (Cascading Style Sheets) is a styling language that describes how elements should be rendered in the browser. CSS modifies the presentation of the HTML code. CSS is the dress up of coding languages.

#### Vocabulary

- CSS
- selectors
- key:value pairs
- pseudo selectors

#### Additional Resources

- [W3Schools CSS](https://www.w3schools.com/w3css/defaulT.asp)
- [CSS Tricks guide to flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Flexbox Froggy](http://flexboxfroggy.com/)
- [Flexbox Defense](http://www.flexboxdefense.com/)
- [CSS Animation for Beginners](https://thoughtbot.com/blog/css-animation-for-beginners)

#### Process

- Create a new file in your project folder called `treasurehunt.css`

#### Troubleshooting Tips

- Is the stylesheet connected to the HTML page?
- Did you save your file?
- Did you refresh your browser?

---

### CSS basics

CSS doesn’t do much without HTML for it to act on, it is the skin covering the skeleton code of HTML. CSS styling can be written once, and used by multiple tags in your HTML code. Creating a styling sheet helps us achieve the coding philosophy of "separation of concerns" which divides responsibility between different areas of your code. It also allows us to be DRY, which stand for Don't Repeat Yourself.

Styling in CSS can be more difficult that you expect, it comes down to a lot of trial and error, don’t be discouraged. There are many wonderful online resources that help with finding the correct CSS attributes.

CSS is set in _key: value_ pairs targeting a particular HTML tag, id, or class.

```css
h1 {
  color: blue;
  font-size: 50px;
}
```

Notice the selector and the curly brackets that surround the _key: value_ pair.

To target a tag's id use the pound sign `#`

```css
#the-id-name-here {
}
```

To target a class use a period `.`

```css
the-class-name-here {
}
```

Particular CSS properties have a shortcut that can be listed together in one key: value pair as long as they are in a particular order.

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

### Treasure Hunt Challenge (CSS)

Create a new file in the `treasure-hunt` folder called `treasurehunt.css`

Add a link tag to the head of the HTML page.

This is an opportunity for you to explore styling. There are many, many possibilities for creating a look for your game, have fun and be creative.

Possible options include:

#### Google fonts

- Select the font you like
- Click the `+` sign
- Copy the link tag from the popup and paste in the HTML head tag
- Copy the CSS _key: value_ pair from the popup and add to CSS file

#### Background image

This is a great description of background image attributes from W3School using the HTML class selector hero-image.

```css
/* The hero image */
.hero-image {
  /* Use "linear-gradient" to add a darken background effect to the image (photographer.jpg). This will make the text easier to read */
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("photographer.jpg");

  /* Set a specific height */
  height: 50%;

  /* Position and center the image to scale nicely on all screens */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

/* Place text in the middle of the image */
.hero-text {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}
```

#### Hover attributes

There is a particular subset of CSS attributes called pseudo selectors. **Pseudo selectors** act on other attributes to make modifications to the styling. A common pseudo selector is the hover attribute that would only show a particular styling when the cursor is over the HTML tag.

Note: this attribute will not behave well on mobile apps as the "cursor" on your phone is your finger or stylus touching the screen.

#### Borders

Centering items using flexbox:

- [CSS Tricks guide to flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Flexbox Froggy](http://flexboxfroggy.com/)
- [Flexbox Defense](http://www.flexboxdefense.com/)

#### Font Colors

CSS recognizes many color names, but to have a more specific hue/shade look for color `#hex` codes.

#### Animation

Animation uses an attribute `@keyframes` that breaks down the total length of your animation into as many frames as you choose. The difference in each frame creates the movement or action.

This website breaks explains each of the animation attributes and gives great examples: [CSS Animation for Beginners](https://thoughtbot.com/blog/css-animation-for-beginners)

[Transform Function](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function)

- `scaleX()` for transforming how wide a selected item is
- `translate()` transforming "where on the page" something is located compared to its original location
- `rotate()` a transformation that rotates an element around a fixed point on the 2D plane
