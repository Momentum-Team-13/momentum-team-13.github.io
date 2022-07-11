---
title: 🐻 Welcome to Advanced Back End 🐻
layout: post
tags: phase-3 back-end
---

### ⚠️ You only need to read this post if you are on the back end team 🐻

## 🗓️ Today's Topics

- Using [PostgreSQL](https://www.postgresql.org/) with Django
- Deploying Django applications to [Heroku](https://www.heroku.com/)

## 🎯 Project: Habit Tracker

You'll be working on [Habit Tracker](https://classroom.github.com/a/vE6TJEWx) this week.

It's important to read the project requirements **thoroughly** and to start to think about how you would do this project.

First steps: generate the project skeleton; make sure you are using Postgres; deploy to Heroku; and design your models. Make sure to create a diagram showing model fields and relationships. _Talk through with each other_ how you are thinking about this.

**By tomorrow**:

- Your application should be **deployed** to Heroku.
- Your **models** should be functional.
- You should be able to create habits and associated daily records in the Django shell (I recommend using `shell_plus` which is available when you have `django-extensions` installed).

## 📖 Read | 📺 Watch | 🎧 Listen

_These are this week's required readings, videos, and/or podcasts. Read, watch, or listen, and **take notes**._

### Deployment

- 📺 [Katie McLaughlin, What is Deployment, Anyway?](https://2021.djangocon.us/talks/what-is-deployment-anyway/)
- 📖 [Full Stack Python: Deployment](https://www.fullstackpython.com/deployment.html)
- 📖 [Heroku Reference: Deploying Django Apps to Heroku](https://devcenter.heroku.com/articles/deploying-python)
    - [Walkthrough: Getting Started with Python/Django Apps on Heroku](https://devcenter.heroku.com/articles/getting-started-with-python)
- 🎧 [Deploying and Running Django Web Apps in 2021](https://talkpython.fm/episodes/show/301/deploying-and-running-django-web-apps-in-2021)

### Databases & Data Modeling

- 📖 [Full Stack Python: Databases](https://www.fullstackpython.com/databases.html)
- 📖 [Full Stack Python: ORMs](https://www.fullstackpython.com/object-relational-mappers-orms.html)
- 📖 [Class-Responsibility-Collaborator Model (CRC)](http://agilemodeling.com/artifacts/crcModel.htm)
- 📺 [Entity Relationship Diagrams (ERD), from Lucid Chart](https://www.youtube.com/watch?v=QpdhBUYk7Kk)
- 📖 [Writing Safe Database Migrations in Django](https://markusholtermann.eu/2021/06/writing-safe-database-migrations-in-django/)

### Debugging

- 📖 [Python Debugging with Pdb](https://realpython.com/python-debugging-pdb/)
- 📺 [Damilare Onajole, Debugging Python](https://pyvideo.org/pycon-nigeria-2018/debugging-python-applications-for-profit.html)

## 🔖 Resources

### Authentication, Registration, and the User Model in Django

- [django-registration-redux](https://django-registration-redux.readthedocs.io/en/latest/index.html)
    - We are using the [simple (one-step) backend](https://django-registration-redux.readthedocs.io/en/latest/simple-backend.html#the-simple-one-step-backend)
- [Django docs: User Authentication](https://docs.djangoproject.com/en/4.0/topics/auth/#user-authentication-in-django)
- [Django docs: built-in User Model](https://docs.djangoproject.com/en/4.0/ref/contrib/auth/#user-model) -> _documentation for all the things you get for free with the User from Django_
- [Django docs: Extending the built-in User Model with AbstractUser](https://docs.djangoproject.com/en/4.0/topics/auth/customizing/#extending-django-s-default-user)
    - [Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model) -> _This tutorial is good to read for an overview, but you don't need to follow the instructions to implement the forms to create or change a user, since we are using the `django-registration-redux` package for that._
- [Django docs: Authentication in Web Requests](https://docs.djangoproject.com/en/4.0/topics/auth/default/#authentication-in-web-requests) -> _`django-registration-redux` handles some of this for us (giving us the login and logout urls, for instance) but it's helpful to see other ways you can use the authenticated user._
- [The `login_required` decorator](https://docs.djangoproject.com/en/4.0/topics/auth/default/#the-login-required-decorator)
- [Limiting access to logged-in users that pass a test](https://docs.djangoproject.com/en/4.0/topics/auth/default/#limiting-access-to-logged-in-users-that-pass-a-test)


- [🚀 Deploying a Django app to Heroku](https://momentumlearn.notion.site/Deploying-a-Django-App-to-Heroku-81488333c03445539bfc7eb3c1691ed0)
- [Using Postgres Locally](https://momentumlearn.notion.site/Using-Postgres-Locally-6d24cd1ea8854eabb875023d6696fba9)
- [Django Docs: Deployment Checklist](https://docs.djangoproject.com/en/4.0/howto/deployment/checklist/)
- [How to use django-extensions `shell_plus`](https://django-extensions.readthedocs.io/en/latest/shell_plus.html#shell-plus)
- [Tutorial: Adding a Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)



## 👾 Code & Notes

- [Example: Django Music configured for auth and postgres](https://github.com/Momentum-Team-13/example-django-music)
