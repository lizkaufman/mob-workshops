# JS 101

## JS as part of a webpage

### Getting Set Up

- Make a new folder and within it an `index.html` that contains the following

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Say Yes to Jay Ess</title>
  </head>
  <body></body>
</html>
```

- Make a new file called `main.js` and within it `console.log` the words "HELLO, WORLD!" like so:

```js
console.log("HELLO WORLD!");
```

- link the JavaScript file to the HTML file with a `script` tag like so:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Say Yes to Jay Ess</title>
  </head>
  <body>
    <script src="main.js"></script>
  </body>
</html>
```

_\* NOTE: script tags are normally placed as the list child/children of the body. This is because the browser will read each line of HTML from top to bottom and most of the time we will want our page to have loaded before we run any scripts._

- Open the HTML page in the browser, open the console and you should see that the words "HELLO, WORLD!" (or your witty own take on the canonical hello world no doubt...) have been printed!

- This means success! We have an HTML page and a JavaScript file, linked and running. Which means it's time to get coding!
