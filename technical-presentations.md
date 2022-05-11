---
title: Technical Presentations
permalink: /presentations/
layout: default
---

# Team Twelve Technical Presentations

- Phase 1: _Thursday, April 14_ 2:00 pm
- Phase 2: _Thursday, May 12_ 2:00pm

Each student will give a short technical talk about a JavaScript project that they worked on during the previous weeks of the phase.

The talk should be 4 minutes long. You'll be speaking to fellow students and instructors. You do not need slides or a script. Just be yourself and tell us about the code you wrote.

The goals of this presentation are:

- To get experience talking about your code, as you will do during interviews
- To demonstrate that you can use the skills taught in the phase to build a dynamic web page or application
- To recognize how much you have learned, to celebrate how hard you’ve worked, and to show your readiness to move into the next phase of your coding education

## Instructions

Choose a project that you've done that shows what you learned during the phase.

- The project should be complete and without errors.

  - _Complete_ means that every feature you started to implement is finished. You may not have gotten to absolutely everything specified in the assignment, but the project is working.
  - _Without errors_ means that nothing in the project is broken and there are no errors in the console.

- **For Phase 1**, the project must include JavaScript, so you can choose anything from week 2 on.
- **For Phase 2**, you can present any Python or Django project
- 
- The size of the project is not important. You should choose a project that you liked doing and that you are excited to talk about.

- You are not expected to sound like an expert or to remember all the right words for everything!

### Your task

1. Explain what the project is. Show it briefly from the user perspective first. What does it do? Tell us about it in plain language (1 min or less).
2. Pick ONE aspect of the project to discuss in more detail (3 min or more) and tell us about the code you wrote to make it work. Please focus on one section of the code and walk us through what it does.

  Some things we'd like to hear you talk about:

- What does this specific code do?
- How does this part of the code work?
- Describe what you did and why you did it that way.
  - How does this provide functionality to the project? Why is it needed?
  - Did you consider doing it a different way or have to make any adjustments to it along the way?
- Point out any interesting parts of this code. Was there something you figured out how to do here that you are proud of? Anything particularly tricky?

You don’t have to read the code to us, but **you should be able to describe how the code works** in terms that your technically skilled audience understands.

**If you are presenting a Django project**

One way to think about presenting is to present one 'page" in the app and talk about its different parts:
- url
- view (probably also involves models)
- template
- form (if used)


## Example

Here’s an example of how you might talk about a project. This example project is a matching tile memory-style game for the browser.

_I built this memory game using HTML, CSS, and JavaScript. If you click on one of these tiles, it flips over to reveal the other side. Then you can click on another tile to see if you’ve found a match._

_The tiles are just divs arranged using flexbox and styled with some simple CSS. I used JavaScript in conjunction with CSS to create the flip effect. Here is the code that does that. On line 14, the event listener on the tile is triggered by a click. In the callback function, I’m adding a class, which applies a CSS animation to the tile that makes it spin and change appearance._

_One interesting thing I figured out for this project is how to compare the tiles to see if they match. The value of the tiles are stored in a data attribute, and they are just strings that correspond to the font icon on the tile. If the tiles match, then the pair is removed from the board. To keep the shape of the board, I don’t remove the elements from the DOM but just set a "hidden" attribute on the tiles that are no longer in play. There are some more animations there to make the effect seem smooth._

_The game ends when all the matches have been found. I show the number of tries that it took to find all the matches, and the user sees an option to play again, which will reset the score and redraw the board. The trickiest part of that was...and here’s how I did it…._

## Evaluation

Your instructors will assess the work you’ve done and determine whether you will go on to the next phase.

The criteria for passing the phase are:

- Your project is complete (meets criteria in the original assignment).

- You can explain how your code works. Instructors may ask you about any portion of it and you can give a reasonable explanation.

You might be asked to repeat the phase if:

- You are unfamiliar with how your code works.

- You have nothing to present.
