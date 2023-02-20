# 💻 JavaScript

#### Overview

JavaScript is a versatile and powerful language in programming. JavaScript is a scripting language, meaning it is used to create logic that will make a webpage react to the interactions from a user. Alongside HTML and CSS, JavaScript is one of the core technologies of the World Wide Web.

#### Vocabulary

- JavaScript
- data type
- number
- string
- Boolean
- variable
- camelCase
- equality operator
- relational operator
- string interpolation
- conditional statement
- function
- parameter
- function invocation

#### Additional Resources

- [JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)
- [JavaScript Built-in Functions Organized By Data Type](https://www.tutorialspoint.com/javascript/javascript_builtin_functions.htm)

#### Process

- Create a new file in your `jumpstart` folder called `javascript-practice.js`
- Open a browser and inspect the page (right click, or control click, in the browser)
- Click over to the next tab called `Console`

#### Troubleshooting Tips

- What data type are you working with?
- Did everything get copied and pasted correctly?
- What does your error say?

---

### JavaScript Fundamentals

**JavaScript** is a dynamic computer programming language that creates interactive experiences with the user.

The Chrome console has a platform to run JavaScript. To access the platform we need to inspect the page. Right click on any page in the Chrome web browser and select the inspect option. At the top you will see a series of tabs. Select the tab called `Console`. This is a JavaScript runtime that will execute your JavaScript code but will not save your work or make any permanent changes.

### Data Types

The building blocks of JavaScript are **data types** which is how we define information for the computer. There are lots of data types but we are going to focus on numbers, strings, and Boolean values.

The **number** data type consist of both full-number integers and partial numbers called floats. Numbers are used for mathematical computations and evaluations.

```javascript
42
3.14
```

The **string** data type is a collection of characters stored in quotation marks. Any data can be stored in a string.

```javascript
"Hello World!"
"42"
```

The **Boolean** data type are the values of `true` and `false`. Booleans are used in evaluations and coding decisions.

```javascript
true
false
```

### Variables

**Variables** are named storage locations. Variables are used to hold data and make data easier to reference in our application.

To create a variable there are four important parts. First we need a variable declaration. A variable declaration tells JavaScript we indeed to create a variable. Next is the name. Variable names should be descriptive and follow the JavaScript naming convention called camelCase. The **camelCase** naming convention starts with a lowercase letter and the first letter of each additional word is capitalized to make it easier to read. The next step is the assignment operator. An assignment operator is a single equal sign. Then the value of the variable can be any data type recognized by JavaScript.

- Declaration: `var`
- Name: `myName`
- Assignment operator: `=`
- Value: `"Jumpstart Student"`

```javascript
var myName = "Jumpstart Student"
```

### Operators and Comparisons

The purpose of JavaScript is to perform logic. There are several different ways we can have our code make decisions.

The first is the equality operator. An **equality operator** determines if two values equate to the same. The operator uses three equal signs and returns a Boolean value.

```javascript
5 === 3 + 2
// true

5 === 3 + 3
// false

var myName = "Jumpstart"
myName === "Jumpstart"
// true
```

**Relational operators** compare whether a values is greater or less than another value. A relational operator returns a Boolean value.

```javascript
// greater than
100 > 5
// true

// less than
30 < 29
// false
```

### String Interpolation

**String interpolation** is a string syntax that allows a variable name to be added dynamically into a string. String interpolation is a collection of characters wrapped in backticks and uses `${}` for the variable.

The backtick button live above the tab button on your keyboard.

```javascript
${variableName}

`This is string that is wrapped in backticks and uses ${stringInterpolation} to drop in a variable.`

var myName = "Jumpstart"
`Hello there, ${myName}!`
// Hello there, Jumpstart!
```

### Conditionals

A **conditional statement** is a sequence of instructions that produce a unique output based on the value of the input. Conditionals follow a flowchart-like structure and allow us to create logic in our code.

The structure sets up a series of statements to be evaluated. Each statement has a corresponding code block that will be executed if the statement is true. Each conditional statement will have exactly one outcome.

```javascript
if(this thing is true) {
  then do this thing here
}
else {
  if the first thing is not true, do this
}
```

- `if`: begins the conditional statement and provides a condition to be evaluated
  - There will only be one `if` in a single conditional statement
- `else if`: follows the `if` and provides an additional condition to be evaluated
  - There can be many `else if` statements
- `else`: catchall that provides an outcome that will run if none of the previous conditions are met
  - There will only be one `else` in a single conditional statement

### Functions

A **function** is a reusable code snippet that performs an action or behavior. Functions can take in information and perform evaluations producing an outcome.

To create a function we have to start with a variable declaration. Earlier when we created variables we used the declaration `var`. To create a function we are going to use the declaration `const`. The declaration `const` will prevent the variable from being reassigned.

Next we need to give our function a name. Just like any other variable, a function should have a descriptive name and be in camelCase. After the name we need an assignment operator.

```javascript
const greeter =
```

After the assignment operator we need parentheses. In JavaScript, parentheses indicate action. Any information that needs to be added to the function can be passed through the parentheses. Passing information into a function requires creating a parameter. A **parameter** is a variable that belongs to a function.

```javascript
// function without a parameter
const greeter = ()

// function with a parameter
const greeter = (name)
```

After the parentheses is the arrow syntax. The arrow syntax indicates the type of function we are creating. Following the arrow will be a code block indicated by curly braces. All the code logic in the function will be inside the curly braces.

```javascript
// function without a parameter
const greeter = () => {
  // code block
}

// function with a parameter
const greeter = (name) => {
  // code block
}
```

Any code logic needed can live inside a function. The ultimate output of the function is indicated by the keyword return. Return is a protected work in JavaScript that is the last thing that happens in any function.

```javascript
// function without a parameter
const greeter = () => {
  return "Hello World!"
}

// function with a parameter
const greeter = (name) => {
  return `Hello ${name}!`
}
```

The function is all ready to go! But the interesting things about functions is that they don't do anything until they are told to. Telling a function to run is called **function invocation** a function. To invoke a function we call the name of the function followed with parentheses.

- Declaration: `const`
- Name: `greeter`
- Assignment operator: `=`
- Parentheses: `()`
- Parameter: `(name)`
- Arrow syntax: `=>`
- Curly braces: `{}`
- Keyword return: `return`
- Function invocation: `greeter("Jumpstart")`

```javascript
// function without a parameter
const greeter = () => {
  return "Hello World!"
}
greeter()

// function with a parameter
const greeter = (name) => {
  return `Hello ${name}!`
}
greeter("Jumpstart")
```

### JavaScript Tips and Tricks

It can be helpful to create a random number in JavaScript. Random numbers will be useful in creating the game play in the treasure hunt game. JavaScript has a code snippet that will produce a random number between 0 and 1. We can multiply this number by any whole number then apply an action that will round the number down to the nearest whole number.

```javascript
// will create a random number between 0 and 3
Math.floor(Math.random() * 4)

// will create a random number between 0 and 7
Math.floor(Math.random() * 8)
```

There is a handy tool in JavaScript for displaying the output of code. This is necessary when creating code in a JavaScript file. To see the outcome of code use `console.log()` and pass in a value into the parentheses.

```javascript
console.log("Hello world!")
// Hello world!
```

There are built in actions in JavaScript called `alert()` and `prompt()` that create interaction with the user. An `alert()` will pop up a message in the web browser. A `prompt()` will create a popup where the user can type information. A `prompt()` can be saved as a variable which will capture the user's input.

```javascript
alert("Hello!")

var favoriteFood = prompt("What is your favorite food?")
```

### Challenge: Greeter

Prompt the user to enter their name. Once the user enters their name alert a greeting.

```javascript
var userName = prompt("What is your name?")

// Alert: "Hello, <name>!"
```

### Challenge: Madlibs of the Amazon

A Madlib is a game where a person is prompted to provide a series of words. Each word is prompted by a particular part of speech. The words are words are substituted for blanks in a story which creates a silly outcome.

Create the code that will prompt the user for a series of words based on the part of speech. Use the result of those prompts to alert a funny story.

"Once upon a time there were some intrepid explorers who wandered into the Amazon. They found some amazing things! Piranhas are more _adjective_ during the day, so make sure you cross the _noun_ at night. Piranhas are attracted to fresh _liquid_ and will most likely take a bite out of your _body part_ if you _verb_. Whatever you do, if you have an open _noun_ try and find another way to get back to _place_. Good luck!"

```javascript
var adjective = prompt("Please enter an adjective.")
var noun1 = prompt("Please enter a noun.")
```

Using string interpolation alert the paragraph with the variables plugged into the story.

### Challenge: World Domination

Create a program that determines the user's ability to rule the world.

- Create a prompt that asks for the user's name.
- Create a prompt that asks the user if they know how to write code.
- If the user replies "yes" respond with an alert that says, "You will rule the world, _name_!"
- If the user does not reply "yes" respond with an alert that says, "Well, good luck with that."

### Challenge: Magic 8 Ball

Create a function that asks the user a question and returns a random answer.

- Create a prompt where the user can ask a question.
- After the user submits a question, create an alert that gives a random answer from the magic 8 ball.
- Traditional 8 ball answers include the following but creative liberties are always encouraged:
  - Better not tell you now
  - It is decidedly so
  - Don’t count on it
  - Signs point to yes
  - Outlook not so good

```javascript
const magic8 = () => {
  prompt("Ask the Magic8 8 Ball a question.")
  var randomNumber = Math.floor(Math.random() * 3)
  ....
}
```

---

### 💎 Treasure Hunt Challenge

- [ ] Create a new file in the `treasure-hunt` directory called `treasurehunt.js`.
- [ ] Add a script tag to the bottom of the HTML body so the HTML page knows it has a dependency. Notice there is no innerHTML.

```html
<script type="text/javascript" src="treasurehunt.js"></script>
```

- [ ] Create a function called `treasure` that returns an alert.

```javascript
const treasure = () => {
  return alert("Here is the function!")
}
```

- [ ] Add an `onclick` attribute to all the game board squares that calls the `treasure` function. If this is done correctly, the alert should appear each time the user clicks on a square.

```html
<td onclick="treasure()">?</td>
```

- [ ] Add a parameter to the function called `location` and pass the location parameter to the alert.

```javascript
const treasure = (location) => {
  return alert(location)
}
```

- [ ] Add a unique id (numbers 0-8) to all game board squares.
- [ ] Pass the same number into the function invocation. If this is done correctly, the alert will display the id of each square.

```html
<td id="0" onclick="treasure(0)">?</td>
```

- [ ] Replace the alert with an action that will change the question mark innerHTML to a tree icon when clicked.
  - We can use the icon symbols or emojis.
  - Access the emoji keyboard by clicking `fn` on a mac or `WindowKey +` for a windows computer.

```
&#x1f332 = tree icon
&#x2620 = bomb icon
&#x1f308 = rainbow icon
```

```javascript
// using the icon symbol
document.getElementById(location).innerHTML = "&#x1f332"

// using an emoji
document.getElementById(location).innerHTML = "🌴"
```

- [ ] Create a variable for the treasure that will store a random number between 0 and 8.
- [ ] Create a variable for the bomb that will store a random number between 0 and 8.
- [ ] Add a conditional statement that will evaluate if the location clicked equates to the random treasure location.
- [ ] If the treasure evaluation is true change the innerHTML question mark to a treasure.
- [ ] Add another level to the conditional statement that will evaluate if the location clicked equates to the random bomb location.
- [ ] If the bomb evaluation is true change the innerHTML question mark to a bomb.
- [ ] Add an `onclick` to the HTML button that will refresh the page, resetting the game board.

```html
<button type="button" onclick="location.reload()">Restart Game</button>
```

Things to consider:

- What if the bomb and treasure are in the same location?
- How does the game end?

Stretch goals:

- [ ] Add a counter to keep track of the number of clicks. The user has a set amount of tries before losing the game.
- [ ] Add multiple bombs.
- [ ] Create a larger map.
- [ ] The user must collect multiple treasures before running out of clicks or clicking on a bomb.
- [ ] Play against the computer
  - Race the computer to find the treasure.
  - Create another function to handle the computer's moves.
  - Create another button on the page to run the computer's turn.
  - Ensure the user cannot keep playing while it's still the computer's turn and vice versa.

---

[Back to the top](#-javascript)

[Back to the main page](../README.md)
