# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks. 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results. 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 

My examples will all refer to how a large organization, such as a professional guild or union, might manage their membership data. 
.map creates a new array based on an existing one by performing some manipulation on each item of the source array. A use case would be creating a call list by selecting only the name and phone number of each record of an organization's membership database. .reduce returns a value based on some agglomeration of information contained in the items of an array. It could be used to deliver the average or total dues owed by members of the organization. .filter creates a new array from the source by including only the items that meet a given condition. It could be used to discover only the organization members whose dates of birth are in the coming week in order to send out a happy birthday message.

2. Explain the difference between a callback and a higher order function.

    A callback function is one that is passed as an argument to another function. The function that makes use of the callback function is called a higher order function. Any function that outputs another function as its return value is also regarded as a higher order function. 

3. Explain what a closure is.

    A closure refers to the context that is encapsulated whenever a function is called. This context can be preserved by assigning a specific instance of the function call to a variable. As long as the variable remains in memory, the context provided at its creation can be recalled. This allows for functionality in javaScript similar to that afforded by 'private variables' in other programming languages. 

4. Describe the four principles of the 'this' keyword.

    1. Window scope - Absent any other contextual information, the 'this' keyword will refer to the widest scope available, in web browsers this is the 'window', in node.js it is called 'Global' scope. Window-scoped 'this' references are to be avoided generally because there is almost never a reason to manipulate the window in this way. 
    2. Implicit binding - When a method of an object is called, 'this' refers to whatever the next highest level of scope would be. This can be determined in dot syntax by looking one spot to the left of the dot in the call. For example, when calling arr.map(), 'this' would refer to the array, 'arr', from which .map is being called. 
    3. Objects created with 'new' - When an object is created by a constructor function using the 'new' keyword, 'this' references inside the constructor refer to the instance of the object that is being created.  
    4. Explicit binding  - Using the functions .call(), .apply(), and .bind() it is possible to explicitly assign the 'this' value for the function being called. 

5. Why do we need super() in an extended class?

    super() allows the child class access to the full set of properties and methods provided in the parent class. It is analagous to the .call(this, attributes) function in pseudoclassical inheritance. 

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your repo to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/master; your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/bloomtech/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://bloomtech.notion.site/bloomtech/BloomTech-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) (see part 2, submitting an assignment with codegrade).
