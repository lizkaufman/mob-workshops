# Make a Quiz

We are going to make a quiz app. It will build upon what we did yesterday as well as adding in arrays.

This task includes

- Arrays
- Loops
- If statements

## Our Plan

- Declare a variable called `currentQuestion` and assign it the value of `0`.
- Declare a variable called `score` and assign it the value of `0`.
- Declare a variable called `questions` and assign it an array of string questions with yes/no or true/false answers.
- Declare a variable called `answers` and assign it an array of answers.
- Within a loop, access an item from the questions array using `currentQuestion` variable and get the user to respond.
- Compare the response with the item at the `currentQuestion` index in the answers array.
- If it matches
  - add one to the score
- Add one to `currentQuestion`
- Loop back and ask the next question.
- Do this until `currentQuestion` is greater than the number of questions.
- Print the score to end the quiz.

## Task

Follow the steps below to implement the above plan. Refer to the logic in [the password checker](../js-101/password-checker.md) if you need to help.
