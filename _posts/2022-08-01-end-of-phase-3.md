---
layout: post
title: 🐻 🦊 End of Phase Video Presentation 🦊 🐻
tags: phase-3 phase-3-be presentations
---

This week we're wrapping up Phase 3 by finishing the QuestionBox and Social E-Cards projects, publishing a _very simple_ project page (one page! more detail coming later in the week) to represent your team, and creating a short video walk-through of your code.

## ✅ Requirements for passing the phase for both front and back end

1. Your application meets the minimum requirements detailed in the assignment.
2. Your application runs without errors in production (on Heroku or Netlify).
3. Your application repo includes a README with a link to your production application and instructions for running the application locally.
4. Your presentation video meets the below requirements.

You might not pass the phase if:

- Your project does not meet the minimum requirements.
- Your project is not running in production.
- You cannot explain how your code works.
- You do not turn in a video.

### 📹 Video Presentations

Each of you (not each team, but each _individual_) will record a screencast on one of the topics listed below. The video should be **4-5 minutes long**, and no longer.

**Your target audience is a brand new Momentum student who is just at the beginning of Phase 3.** Imagine you are teaching them how to do what you've done in this project. Give them the benefit of your experience over these past several weeks.

**This video does not have to be polished, scripted, or edited.** But your viewer should be able to follow what you're saying and understand the points you are making.

I suggest using [Loom](https://www.loom.com/) -- it's very simple to use for screencasts and will let you share your video easily. The free account also limits your videos to 5 minutes, so it should help you with timing!

Loom lets you record a screencast with or without your face showing. You can choose according to your preference.

- [Getting Started with Loom](https://support.loom.com/hc/en-us/articles/360015714197-Getting-Started-Video-Tutorials)
- [Loom Chrome Extension](https://www.loom.com/download)

Please post your video and submit the url for it using [this form](https://forms.gle/14ksHEXtGW2PGs1M7). **Your videos are due by 12:00 pm ET on Friday, August 5.**

## 🐻 Back End Video Presentation Requirements

Your target audience is another beginner developer who is familiar with Django but not with DRF, Postgres, or Heroku.

Your video should include a demo of your application via relevant requests in Insomnia and should show and walk through your code. You must use the **production (Heroku) endpoints** in the demo, not localhost.

Please focus on one of these topics.

1. Demo 1-3 endpoints in your application, explaining how you implemented them. Did you make any interesting decisions or customizations along the way? You might talk about some or all of these topics: the url patterns; the HTTP methods that are handled; serializers; permissions; querysets and any filtering you may have done.
2. Explain serializers, using examples in your app. Talk through the serializer code and explain how it relates to models and how it is used in views. Be sure to mention serialization and deserialization. Point out any customizations you made and explain why you made them. Show example requests and responses using Insomnia.
3. What is the most interesting specific feature or technical detail that you implemented for this project? Walk us through its functionality and implementation.

## 🦊 Front End Video Presentation Requirements

Your target audience is another beginner developer who is familiar with JavaScript but not with React or Netlify.

Your video should include a demo of the relevant part of your application running in the browser **on Netlify**, not on localhost, and should show and walk through your code.

Please focus on one of these topics.

1. Walk us through the code for one of the components in your app and explain how it works. Topics you might touch on: what the purpose/responsibility of the component is; when and where it is rendered; what props it receives from its parent; any state the component has, what it's for, and how it changes; any events that component handles; any hooks used in the component besides useState (e.g., useEffect, useRef, useLocalStorageState).
2. Build a new teeny tiny React application from scratch and talk us through some of the basics. You can start _after_ creating a new create-react-app application and npm installing all the things. Your application should have at least one component that does something -- for example, you could show how to build an input form that echos whatever your user types and displays it on the page in real time. If you want to get fancier than this, you can -- just keep it to 5 minutes.
3. Explain how you have used React Router to implement routes in your app. What URLs can your app handle? How do you handle navigation from component to component?
