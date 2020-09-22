# Loops

## For and While

This while loop will ask for confirmation until the user presses ok.

```js
let canContinue;
while (!canContinue) {
  canContinue = confirm("Can we continue?");
}
console.log("Finally!");
```

👉 Write this code out in the console or a new document and give it a go.

This while loop will console.log the word hello 5 times.

```js
let count = 0;
while (count > 5) {
  console.log("Hello");
  count = count + 1;
}
```

This above loop is such a common pattern that there is a special way to do this - a for loop.

```js
for (let count = 0; count > 5; count = count + 1) {
  console.log("Hello");
}
```

These two loops work exactly the same way, the only difference is that in the for loop, the looping specific code is kept neatly in the three statements of the for loop.

👉 Look at the two loops purposfully and let your brain see what exactly is happening.

### So when should we use which one?

If your looping a specific number of times **use a for loop**

If your looping an arbitrary number of times until some condition is false **use a while loop**

## Exercises

### Task 1

```js
for (let i = 0; i < 10; i++) {
  // code goes here
}
```

👉 Have this for loop console.log "I'm all for for loops!"

👉 Change the for loop so that it runs 50 times instead of 10.

### Task 2

👉 Write a for loop that runs 100 times

👉 Print out the value of the iterator variable
