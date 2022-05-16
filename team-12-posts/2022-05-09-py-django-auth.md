---
layout: post
title: 🌦️ 🍃 🌸 🌱 Spring of Django 🌦️ 🍃 🌸 🌱
tags: phase-2 django registration authentication login
---

You've now seen how to handle data in a Django application with basic operations in these CRUD categories:

- **Create** - when we add a new model instance to the database
- **Read** - when we query the database to look up existing data
- **Update** - when we query the database to find existing data so we can change it
- **Destroy** - when we find existing data in the database and delete it

At the heart of many web applications you'll find variations on this theme, so we'll continue to practice it.

Today we'll add in another essential part of web applications: **user registration and login**. This will allow us to create users for our application, let them log in (and out) and associate data with specific users.

## 📋 Django Music Project Review

- 😲 What was one AHA! moment you had?
- ⏲️ What did you spend the most time on?
- 😕 What is something that you'd like to understand better?
- 📝 What are three goals that you have set for yourself for this next assignment?

## 🎯 Project: Django Freeshelf

This is a 3-day assignment that you'll work on this week. It is due on Thursday Morning, May 12. We will do end-of-phase presentations in the afternoon. 

[📚 Django Freeshelf](https://classroom.github.com/a/vqRWfN7R)

## 🔖 Resources

- [Rebecca's Django Videos](https://loom.com/share/folder/721b7feffe124c4fa9b32eed6940610b)

### Authentication, Registration, and the User Model in Django

- [django-registration-redux](https://django-registration-redux.readthedocs.io/en/latest/index.html)
    - We are using the [simple (one-step) backend](https://django-registration-redux.readthedocs.io/en/latest/simple-backend.html#the-simple-one-step-backend)
- [Simple Is Better Than Complex: How to Extend the Django User Model](https://simpleisbetterthancomplex.com/tutorial/2016/07/22/how-to-extend-django-user-model.html)
  - Clear comparison of the four choices you have, and when you would use each one.
- [Django docs: User Authentication](https://docs.djangoproject.com/en/4.0/topics/auth/#user-authentication-in-django)
- [Django docs: built-in User Model](https://docs.djangoproject.com/en/4.0/ref/contrib/auth/#user-model) -> _documentation for all the things you get for free with the User from Django_
- [Django docs: Extending the built-in User Model with AbstractUser](https://docs.djangoproject.com/en/4.0/topics/auth/customizing/#extending-django-s-default-user)
    - [Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model) -> _This tutorial is good to read for an overview, but you don't need to follow the instructions to implement the forms to create or change a user, since we are using the `django-registration-redux` package for that._
- [Django docs: Authentication in Web Requests](https://docs.djangoproject.com/en/4.0/topics/auth/default/#authentication-in-web-requests) -> _`django-registration-redux` handles some of this for us (giving us the login and logout urls, for instance) but it's helpful to see other ways you can use the authenticated user._
- [The `login_required` decorator](https://docs.djangoproject.com/en/4.0/topics/auth/default/#the-login-required-decorator)
- [Limiting access to logged-in users that pass a test](https://docs.djangoproject.com/en/4.0/topics/auth/default/#limiting-access-to-logged-in-users-that-pass-a-test)

### Related Python & Django resources

- [RealPython: What is a decorator?](https://realpython.com/primer-on-python-decorators/)
- [Python dependency management overview](https://modelpredict.com/python-dependency-management-tools) -> _A good read to understand `pip`, `pyenv`, and `pipenv` better._
- [💥 Django Cheatsheet!](https://github.com/lucrae/django-cheat-sheet)
- [💫 Django Chat Podcast: How Django Experts Think](https://djangochat.com/episodes/how-django-experts-think) -> _Worth a listen, especially if you're feeling discouraged about ever learning Django, and super relevant._

## 🦉 Code & Notes

- [Example app: Django Music](https://github.com/Momentum-Team-12/example-django-music)
