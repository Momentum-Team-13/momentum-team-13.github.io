---
layout: page
title: Django Models and Queries
date: 2022-07-12
topic: Python
category: phase3-be
parent: Phase 3 Advanced Back End
nav_order: 2
---

## 🗓️ Today's Topics

- The woes of deployment and what to do about them
- Django managers, lookups, and querysets
- Using the Django shell to test out your models and make queries

## 🎯 Project: Working on Habit Tracker

Today your models should be done, so you can begin building out the urls, views, and templates you will need. Before you write the code, plan for what you will need. A good way to do this is to sketch out what your user will see.

There are examples for a lot of what you need to do in the Django Recipes codebase but you will have to adapt them to your Habit Tracker use cases.

## 🔖 Resources

### Models

- [List of all Django Reference content related to Models](https://docs.djangoproject.com/en/3.2/ref/models/)
- [Don't forget! Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)
- [Django Docs: Saving Model Instances](https://docs.djangoproject.com/en/3.2/ref/models/instances/#saving-objects)

### Managers and QuerySets

- [Django Model Managers](https://docs.djangoproject.com/en/4.0/topics/db/managers)
- [Django Related Objects Reference](https://docs.djangoproject.com/en/4.0/ref/models/relations/#related-objects-reference)
- [Django QuerySets](https://docs.djangoproject.com/en/4.0/topics/db/queries/#retrieving-objects)

### Queries

You can think of queries as talking to the database. To support all our CRUD actions, we need to be able to create, read, update, and delete objects from the database. Django has a built-in library (the Django ORM) that lets us do all that.

- [Django Queries: Retrieving Objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#retrieving-objects)
- [Django Queries: Field lookups](https://docs.djangoproject.com/en/4.0/topics/db/queries/#field-lookups)
- [Django Queries: Lookups that span relationships](https://docs.djangoproject.com/en/4.0/topics/db/queries/#lookups-that-span-relationships)
- [Django Queries: Lookups with Related objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#related-objects)

## 🌟 EXTRA/TMI

- [SQL Basics: Learn X in Y minutes](https://learnxinyminutes.com/docs/sql/) -> this is a helpful reference for SQL syntax when you run into it. You do not need to write SQL for Django because the Django ORM does it for you, and it does it well. The Django docs often illustrate queries made by the ORM using SQL syntax, however, and you will find it helpful in your job to know the basics.
- [Postgres GUI: Postico](https://eggerapps.at/postico/)

## 🦉 Code & Notes

- [Deploying a Django App to Heroku](https://momentumlearn.notion.site/Deploying-a-Django-App-to-Heroku-81488333c03445539bfc7eb3c1691ed0)
- [Using Postgres Locally](https://momentumlearn.notion.site/Using-Postgres-Locally-6d24cd1ea8854eabb875023d6696fba9)
- [⭐ Django Queries Cheat Sheet](https://github.com/Momentum-Team-13/notes/blob/main/django-queries.md)
- [Example: Django Recipes App](https://github.com/Momentum-Team-13/example-django-recipes)
