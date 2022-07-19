---
layout: post
title: 🦊 Multiple Components and Conditional Rendering 🦊
tags: phase-3 phase-3-fe react components
---

## 🗓️ Today's Topics

- Getting data on the page with AJAX
- Troubleshooting AJAX requests
- Using multiple components and conditional rendering to create multiple views of your application

## 🎯 Project: React Trivia

This project is due next Monday.

[React Trivia](https://classroom.github.com/a/isanC-ma). Your goal today is to get a list of trivia categories showing on the page.

Remember to take it step by step! Don't try to do too much at once.

Goals in the order you should tackle them:

1. Get a list of categories from the Trivia API showing up on the page.
2. Make your trivia categories selectable. When a user clicks on a category to select it, you should make a request to get at least 10 questions for that category (note: the API will let you specify how many questions you want to get back and it will let you specify the type -- you can limit to the multiple type choice to make it a little easier).
3. If you can get all the questions for the selected category, the next step is to show the questions. Ideally you want to show one question at at a time with answer choices for that question.
      - If this is too hard, just show the first question to start with.
      - Next, show the answer choices for that question (don't worry about the order at first; you can change that later)
      - When you can show one question with its answer choices, then make it possible for the user to see the next question in the list of questions by clicking a button
4. Make it possible for the user to select their answer choice. You will need to know what answer they selected, and you will need to know the correct answer. They got the answer right if the answer they selected is the same as the correct answer (so you'll need to compare those two values somehow).
5. Tell the user if they got the question right.
      - OR keep track of questions answered correctly and tally them at the end (something like, "You got 6 out of 10 questions right!").
6. Have a way for the quiz to end and optionally go back to the list of categories to start another quiz.

Don't skip steps! They build on each other. You may find that you need to break these steps down even further, and that is OK. Make this as easy as you can on yourself!

**By Thursday** you should aim to have the first three goals done -- or at least, the first two and the third in progress.

## 🔖 Resources

- [Using the Effect Hook](https://reactjs.org/docs/hooks-effect.html)
- [React Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)
- [5 Ways to Implement Conditional Rendering in React](https://blog.bitsrc.io/5-ways-to-implement-conditional-rendering-in-react-64730323b434)
- [Lifting State Up](https://reactjs.org/docs/lifting-state-up.html) -- This is the official doc page. To see it with hooks, watch the video [Lifting State Up with Hooks](https://www.youtube.com/watch?v=HF4o9KAZNxw).


## 🦉 Code & Notes

- [React Devs for Hire App](https://github.com/Momentum-Team-13/example-react-devs)
