# HTML

HTML (Hypertext Markup Language) is the computer language that displays information to the user in a web browser.

### To create HTML computer code

- Text editor – at LEARN VS Code
- Save a file with the extension .html (example: index.html)
- Don’t use spaces or capital letters while naming directories or files
- Setup the basic tags needed for your page called the DOCTYPE

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

### HTML tags

- HTML uses "tags" that are indications to the computer what information to display and how it should look
- A tag is surrounded by carrots `< >`
- A set of tags will open `<div>` and close `</div>`
- The text inside the opening and closing tags is displayed in the browser, this is called the innerHTML
- Attributes are extra pieces of information stored inside the opening tag to modify how the browser displays information
- Tags that just store information (like images) don’t have to close, these are called meta tags

```html
<body>
  <h1>Treasure Hunt Game</h1>
  <img src="https://www.picture-url.png" alt="description of picture here" />
  <!-- additional code here! -->
</body>
```

### HTML Code

- The entirety of the code that appears on the page is nested in the `<body> </body>` tags in the HTML DOCTYPE
- Indentation matters!
- Save your work often (command + s)
- Drag the icon in the top of your text editor window into Google Chrome to view your page
- If you make changes to your code you must refresh the browser (command + r)

### Treasure Hunt Challenge (HTML)

- Decide on a theme for your game
  Create a new directory (folder) on your desktop called `treasure-hunt`
- Create a new HTML file in your treasure-hunt directory called `index.html`
- Set up the HTML boilerplate
- Add a header and subheader to your game
- Add a title to the browser tab
- Make a list of the game rules, for example:
  - Click the boxes to reveal what’s on the map
  - If you click on the bomb, you lose
  - If you click on the treasure, you win
  - Add an image tag with a picture to decorate your page
- Make a table to create the game board
  - tr – table row, nested inside the table
  - td – table delimiter, nested inside each table row
- Create a button to restart the game (your button will be useless for today, functionality will come later)
- Add a footer to the page with your names `<footer> </footer>`
- Add a link to the footer to take your user to an external website
- Add a favicon to the browser tab

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>Treasure Hunt Game</h1>
    <img src="https://www.picture-url.png" alt="description of picture here" />
  </body>
  <table>
    <tr>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
  </table>
  <button type="button">Restart Game</button>
</html>
```
