# 04 Web APIs: Code Quiz

As you proceed in your career as a web developer, you will probably be asked to complete a coding assessment, which is typically a combination of multiple-choice questions and interactive challenges. Build a timed code quiz with multiple-choice questions. This app will run in the browser and feature dynamically updated HTML and CSS powered by your JavaScript code. It will also feature a clean and polished user interface and be responsive, ensuring that it adapts to multiple screen sizes.

## User Story

```
AS A coding bootcamp student
I WANT to take a timed quiz on JavaScript fundamentals that stores high scores
SO THAT I can gauge my progress compared to my peers
```

## Acceptance Criteria

```
GIVEN I am taking a code quiz

WHEN I click the start button
  THEN a timer starts and I am presented with a question
WHEN I answer a question
  THEN I am presented with another question
WHEN I answer a question incorrectly
  THEN time is subtracted from the clock
WHEN all questions are answered or the timer reaches 0
  THEN the game is over
WHEN the game is over
  THEN I can save my initials and score
```

The following animation demonstrates the application functionality:

![code quiz](./Assets/04-web-apis-homework-demo.gif)


### Hints

* Store your questions as an array of objects in your `index.js`, that follows this format:

```js
var questions = [
  {
    title: "Commonly used data types DO NOT include:",
    choices: ["strings", "booleans", "alerts", "numbers"],
    answer: "alerts"
  },
  {
    title: "The condition in an if / else statement is enclosed within ____.",
    choices: ["quotes", "curly brackets", "parentheses", "square brackets"],
    answer: "parentheses"
  },
  ///etc.
];
```

* The length of the array in `index.js` determines the length of play. Fifteen seconds per question is a good estimate, so 5 questions will result in a length of play of 75 seconds.


### Review

You are required to submit the following for review:

- The URL of the functional, deployed application.

- The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

---

© 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.



var quizQuestions = {
    
    question1: {
        prompt1: 'What does HTML stand for?',
        optionA: 'html stands for hyper-text-mark-up-language',
        optionB: 'some answerB',
        optionC: 'some answerC',
        optionD: 'some answerD',
    },
    question2: {
        prompt2: 'Some question 2!!',
        optionA: 'some answerA.2',
        optionB: 'some answerB.2',
        optionC: 'some answerC.2',
        optionD: 'some answerD.2'
    },
    question3: {
        prompt3: 'also some question 3!',
        optionA: 'some answerA.3',
        optionB: 'some answerB.3',
        optionC: 'some answerC.3',
        optionD: 'some answerD.3'
    }
}


// for ( var key in quizQuestions){
//     console.log(quizQuestions[key]:${value})
// }
for (let [key, value] of Object.entries(quizQuestions)) {
    console.log(`${key}: ${value}`);
  }