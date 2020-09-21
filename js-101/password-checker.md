# Password Protected

We are going to use our newfound javascript knowledge to make some information only available to people who know the password.

We will use...

- variables
- if statements
- loops
- functions

## Our Plan

- prompt the user for input - a password in our case
- store that password in a variable for future use
- check whether the password matches the correct password
  - if it does, reveal the information
  - if it doesn't let them try again
  - if they fail three times in a row, do not allow them any more tries

## Step 1 - Getting user input

We will the using `prompt` to "prompt" the user for an input

```js
prompt("Please enter the password.");
```

We hand in what we want the prompt to say as an argument, and prompt returns us what the user inputted. At the moment we are not doing anything with the return value of `prompt`.

👉 Use the above code, but change it so that we save the return value in a variable\*.

_\*to check that this step is working, console.log the variable you have made to see if it contains what you've inputted_

## Step 2 - Using the input to determine behavior

Now that we have the user's input stored in a variable, we can check whether it is the correct password. If it is correct, we should then `alert` with some secret information.

```js
alert("My secret information");
```

To check that our variable is equal to the correct password we can use `===`, the equality operator.

```js
userPassword === "myPassword1!";
```

The code above will resolve to true if the variable `userPassword` contains the string "myPassword1!".

👉 Use an if statement to `alert` your message only when the password is correct.

## Step 3 - try again!

We now want to let the user try again if the answer they entered was incorrect, but only for three times.

We can have the code loop round the part where we ask for the password using a while loop.

```js
while (condition) {
  // ask the user for the password
  // give secret and break the loop if correct
}
```

We only want to repeat our loop if the previous guesses are less that three.

This means we will need to keep track of the number of attempts.

👉 Declare a variable at the top of our code called `attempts` with the value of `0`. We will add one to this variable each time the user makes an incorrect guess.

👉 Use the variable `attempts` in the condition of the while loop. We want the while loop to run as long as attempts are less than 3.

👉 If the user enters the wrong password, we want to add 1 to the attempts variable. If they are correct we want to exit the loop.

## Step 4 - Functions

### New Plan

- declare a function that will prompt the user for input - a password in our case
  - store that password in a variable within the function
  - check whether the password matches the correct password
    - if it does, return true from the function
    - if it doesn't let them try again
    - if they fail three times in a row, do not allow them any more tries and return false from the function
- console.log a secret _only_ if the function returned true

👉 Refactor the code you have written into a function called authenticateUser. Have that function return true if the user logged in successfully, and false if they got the password wrong more than three times. You can put most of the code you have written into the function, but don't reveal the secret yet. The function should be used like this...

```js
function authenticateUser() {
  // prompt for password and handle login attempts here
}
// get answer here
let isLoggedIn = authenticateUser();

// you should reveal the secret after the function is called using the boolean isLoggedIn
```

## Step 5 - The End

Well done, you've successfully implemented a password checking system. Hopefully your secret information wasn't too embarrassing and your password was strong enough to keep it secret!

Next steps...

- Split up the functionality into more functions
  - each function should only do one thing
- Let the user know how many attempts they have left.
- Delete the code (or parts of) and practice remembering what you did and writing it out again, this will really help embed your new skills.
- Let your imagination run wild and make something else using the same logic.
