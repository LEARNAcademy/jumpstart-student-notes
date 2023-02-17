# JavaScript

- [JavaScript Practice Exercises](#javascript-practice-exercises)
-

JavaScript is a dynamic computer language that creates interactive experiences with the user.

### JavaScript basics

- Chrome console has a platform to run JavaScript
- Inspect the page (right click in the browser)
- Click over to the next tab called `Console`

### Data types

Data types are how we define information for the computer. There are lots of data types but we are going to focus on three of them.

- Number - integer, float
- String - any information stored in quotation marks `" "`
- Boolean - `true` and `false`

### Variables

Variables are empty buckets that hold information.  
Four important parts:

- Declaration: `var`
- Name: `myName`
- Assignment operator: `=`
- Value: `"Jumpstart Student"`

```javascript
var myName = "Jumpstart Student"
```

### Equality operators

Three equal signs is strict equality evaluations that returns a Boolean value.

```javascript
===
```

### Comparison operators

```javascript
// greater than
100 > 5
// less than
15 < 30
// returns a Boolean value
```

### String interpolation

A string syntax that allows a variable name to be added into a string. String interpolation is a string wrapped in backticks and uses `${}` for the variable.

The back tic button live above the tab button on your keyboard.

```javascript
${variableName}

`A string that has back tics and ${stringInterpolation}`
```

### JS protected words

JavaScript has vocabulary words and actions built in to the language.

```javascript
// reserved words
var
const
function
if
else if
else
return

// built in methods
.alert()
.prompt()
.toLowerCase()
.getElementById()
```

### Conditionals

A conditional is a way to make decisions in your code.

This is the structure:

```javascript
if(this thing is true) {
  then do this thing here
}
else {
  do this thing here
}
```

- `if`: begins the conditional statement and provides a condition that could be met
  - There will only be one if in a single conditional statement
- `else if`: follows the if and provides an additional condition that could be met
  - There can be many else if statements
- `else`: catchall that provides an outcome that will run if none of the previous conditions are met

### Functions

Reusable instructions that can take in information and evaluate the information using code.

Functions have eight parts:

- Variable declaration: `const`
  - This allows us to name our function and not have the program we write get changed by anything else
- The function name: `myFunction`
  - Name your functions something related to what you want them to do
  - Always use camelCase
- Assignment operator: `=`
  - The single equal symbol sets the name we make to the value of of our program
- The parentheses: `()`
  - These parentheses can also take a placeholder depending on what our function wants to do with them
    (number)
    (string)
    (name)
- The arrow: `=>`
  - The arrow => is the part of our program that is actually the function
  - The arrow tells JavaScript "Hey this is a little machine here"
- The curly brackets (code block): `{ }`
  - Any code that we could write in JavaScript can go between these curly brackets
  - These code inside the brackets will only operate when the function is called
- The keyword return: `return`
  - The `return` is the last thing that happens in any function - it will end the function action
  - The return is what the function gives back to you when you call it
  - If you have conditional statements (if/else) you can have one return per conditional statement
- The function invocation: `myFunction()`
  - Outside of the function code using the name of the function and giving it parentheses will let JavaScript know that is the time to use the function code

### JavaScript Practice Exercises

- Open your text editor
- Save a new file inside of the `treasure-hunt` directory called `practice.js`
- Remember: no spaces or capital letters
- Copy and paste your code into the Chrome browser's console to see it run
- Right click the Chrome page and select inspect
- Navigate to the console tab
- You may need to hit return once you have pasted it

### MadLibs of the Amazon

"Once upon a time there were some intrepid explorers who wandered into the amazon. They found some amazing things! Piranhas are more _adjective_ during the day, so make sure you cross the _noun_ at night. Piranhas are attracted to fresh _liquid_ and will most likely take a bite out of your _body part_ if you _verb_. Whatever you do, if you have an open _noun_ try and find another way to get back to _place_. Good luck!"

Premise – write a program that uses the built-in `alert()` method to get people excited
Greeter – write a program using a prompt, saved as a variable, that asks for your name, then says hello to you

```javascript
var yourName = prompt("Please enter your name")
// --> "Hello <yourName>! Let’s go explore the Amazon."
```

Write a program that tells you a funny story.

- As a user, I see a series of prompts that asks me for an adjective, a noun, a liquid, a body part, a verb, noun, and a place
- As a user, I see an alert of a funny story that includes my answers

```javascript
var adjective = prompt("Please enter an adjective.")
var noun = prompt("Please enter a noun.")
```

Etc….

Using string interpolation to refactor the below paragraph so that it displays the values of the variables.

"Once upon a time there were some intrepid explorers who wandered into the amazon. They found some amazing things! Piranhas are more _adjective_ during the day, so make sure you cross the _noun_ at night. Piranhas are attracted to fresh _liquid_ and will most likely take a bite out of your _body part_ if you _verb_. Whatever you do, if you have an open _noun_ try and find another way to get back to _place_. Good luck!"

### World Domination

Create a program that determines the user’s ability to rule the world.

- As a user, I can see a prompt that asks me my name
- As a user, I can see a prompt that asks me if I know how to write code
- As a user, if I reply "yes" I will see the alert, "You will rule the world, _name_!"
- As a user, any reply other than "yes" will alert, "Well, good luck with that."

### Magic 8 Ball

Create a function that asks the user a question and returns an answer.

- As a user, I see a prompt where I can ask a question
- As a user, I see an alert that tells me a random Magic 8 Ball answer
  - Better not tell you now
  - It is decidedly so
  - Don’t count on it
  - Signs point to yes
  - Outlook not so good

### World Domination - Refactor

Take your “World domination” code and refactor it (make changes to the code) so that it is contained in a function.

- As a user, I can run the world domination program by invoking the name of the function

### Treasure Hunt Challenge

Create a new file in the `treasure-hunt` directory called `treasurehunt.js`.

Add a script tag to the bottom of the HTML body so the HTML page knows it has a dependency. Notice there is no innerHTML.

```html
<script type="text/javascript" src="treasurehunt.js"></script>
```

As a first step to connecting the HTML and JS, create a function called `treasure` that takes an argument of `location` and returns an alert displaying the id of the square on the game board when it is clicked on.

Add an `onclick` attribute to all the nested table tags so when our user clicks on the question mark it will trigger the `treasure` function to run in the JavaScript file.

Add a unique id (numbers 0-8) to all `<td></td>` tags so we can identify which `td `was clicked and perform an action on the correct location.

WITHIN YOUR JS FILE: Set up a variable to store the random location of the rainbow treasure

WITHIN YOUR JS FILE: Set up a variable to store the random location of the bomb

WITHIN YOUR FUNCTION: Add a conditional statement that will alert either the location of the bomb, the location of the treasure, or the id. (You may want the “id” alert to tell you the location of the treasure and bomb for troubleshooting purposes)

WITHIN YOUR FUNCTION: Replace the alert with an action that will change the question mark in the td innerHTML to the tree, bomb, or treasure icon. You can also access an emoji keyboard by clicking `control + command + space` on a Mac, Windows . for PC.

```
&#x1f332 = tree icon
&#x2620 = bomb icon
&#x1f308 = rainbow icon
```

Add an `onclick` to the button that will refresh the page, resetting the game board.

Things to consider:

- What if the bomb and treasure are in the same location?
- How does the game end?

Stretch goals:

- Add a counter
  - Set up the counter to keep track of the number of clicks. The user has a set amount of tries before losing the game
  - Assign a variable to the base value
    0
  - Reassign the variable every time the treasure function runs
  - Attach the counter to the HTML with an id tag
- Add multiple bombs
- Create a larger map
- Collect multiple treasures
  - The user must collect all the treasures before running out of clicks or clicking on a bomb
- Play against the computer
  - Race the computer to find the treasure
  - Create another function to handle the computer’s moves
  - Create another button on the page to run the computer’s turn
  - Ensure the user cannot keep playing while it’s still the computer’s turn and vice versa
