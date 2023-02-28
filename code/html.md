# 💻 HTML

#### Overview

HTML (Hypertext Markup Language) is basis of all things on the internet. HTML is the computer language that displays information to the user in a web browser.

To create HTML we will need a text editor. A text editor is the software platform used to write code. We welcome all different text editors, but if you don't have a preference we recommend VS Code.

#### Vocabulary

- HTML
- tag
- innerHTML
- self-closing tags
- attribute
- file extension
- boilerplate HTML
- nested tags
- dependency

#### Additional Resources

- [HTML Boilerplate](https://www.freecodecamp.org/news/basic-html5-template-boilerplate-code-example/)
- [W3Schools HTML](https://www.w3schools.com/html/)

#### Process

- Create a new folder called `jumpstart`
- Create a new file called `index.html`
- Save a file on a mac: `command + s`
- Save a file on a windows machine: `control + s`
- Refresh a browser on a mac: `command + r`
- Refresh a browser on a windows machine: `control + F5`

#### Troubleshooting Tips

- Is your file saved?
- Did you refresh your web browser?
- Quit your browser and reopen.

---

### HTML Fundamentals

Hypertext markup language is the foundation of everything on the internet. **HTML** is a standard markup language that described the structure of all web pages.

The building blocks of HTML are called tags. A **tag** is a snippet of code that gives instructions to the computer on how to display content. A tag is surrounded by carrots `< >`.

There are two categories of HTML tags. The first category has separate opening and closing tags. Inside the tags is the content that is displayed in the browser. This is usually the text we see on the screen. The text content displayed on the browser is called **innerHTML**.

```html
<!-- a header tag with innerHTML -->
<h1>Hello World!</h1>
```

The second category of tags are called self-closing tags. **Self-closing tags** are tags that don't display text and therefore don't have any innerHTML.

Tags can be modified by adding additional information called **attributes**. Attributes sit inside the tag and modify the presentation or behavior of the tag.

```html
<!-- a header tag with innerHTML -->
<h1>Hello World!</h1>

<!-- a header tag with attributes -->
<h1 id="heading">Hello World!</h1>

<!-- an image tag without innerHTML -->
<img />

<!-- an image tag with attributes -->
<img src="www.img.jpg" alt="description of image" />
```

### Creating HTML

Inside the project folder create a new file called `index.html`. Is in important not to use spaces or capital letters while naming directories (also called folders) or files. The **file extension** `.html` informs the computer what type of information to expect in the file. The correct file extension will enable your text editor to give you hints and suggestions to make your coding easier and faster.

Next we need to set up the base structure that exists on every HTML page. This is a set of basic tags needed for your page called the DOCTYPE. This is **boilerplate HTML** code and can be accessed by typing `html` into your text editor and selecting the prompt.

The boilerplate will look something like this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### HTML Code

The boilerplate HTML code will have one tag that wraps the entire file. This is the `html` tag. The `html` tag has two nested tags. **Nested tags** are HTML tags that live inside other HTML tags. This is a common structure and necessary to creating complex HTML. Inside the `html` tag are two additional nested tags. One is the `head` tag. The `head` tag contains information about the page as well as any dependencies. A **dependency** is additional information needed to make the page behave and display correctly. The other tag is the `body` tag. The entirety of the code that appears on the browser page is nested in the `<body> </body>` tags.

Nested tags need to be indented. This provides clarity and keeps code organized.

### Seeing Code in the Browser

Be sure to save the code often. Use keyboard shortcuts to make the process efficient.

Once the file is saved, the file can be opened in the Chrome browser. Each time we make changes to the code we need to be sure to save the file and refresh the browser.

---

### 💎 Treasure Hunt Challenge

First, chat with your pair programming partner and decide on a theme for your game.

- [ ] Add a header and subheader to your game
- [ ] Make a list of the game rules, for example:
  - Click the boxes to reveal what’s on the map
  - If you click on the bomb, you lose
  - If you click on the treasure, you win
- [ ] Add an image tag with a picture to decorate your page
- [ ] Make a table to create the game board
  - `table` - tag that wraps the entire table
  - `tr` – table row, nested inside the table
  - `td` – table delimiter, nested inside each table row
- [ ] Create a button to restart the game (your button will be useless for today, functionality will come later)
- [ ] Add a footer to the page with the names of the developers on the project `<footer> </footer>`
- [ ] Add a link to the footer to take your user to an external website
- [ ] Update the title in the browser tab
- [ ] Add a favicon to the browser tab

Below is an example of creating well-organized, nested tags.

```html
<body>
  <h1>Treasure Hunt Game</h1>
  <img src="https://www.picture-url.png" alt="description of picture here" />
  <hr />
  <table>
    <tr>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
  </table>
  <button type="button">Restart Game</button>
  <footer>&copy; Sarah & Tricia</footer>
</body>
```

---

[Back to the top](#-html)

[Back to the main page](../README.md)
