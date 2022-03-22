---
layout: post
title: 🔎 Django Search 🕵️‍♂️
tags: phase-2 django search query-params
---

## 🗓️ Today's Topics

- Checking in on Code Snippets and Flashcards progress
- Git collaboration review & questions
- Django review & questions
- Implementing search
- Foreign key recursive relationships

## 🎯 Project: Code Snippets | Flashcards

Keep on with your end-of-phase project. Today you should have:

- Models that you can use in the shell and in your application
- At least the urls and views to support the CRUD functionality your application needs
- A complete list of tasks you still need to do, based on the project requirements
- A plan for when you will do them and who will work on them

## 🔖 Resources

### Django Views

- [Django Views: the Right Way](https://spookylukey.github.io/django-views-the-right-way/) _This is a very opinionated and detailed article that goes into a lot of detail about function-based views._
- [Creating Interactive Views in Django](https://hackersandslackers.com/creating-django-views/) _Detailed post really breaking down views._


### Debugging

- [Django Debug Toolbar docs](https://django-debug-toolbar.readthedocs.io/en/latest/)
- [RealPython Debugging with Pdb](https://realpython.com/python-debugging-pdb/) _The built-in Python debugger (Pdb) lets you set breakpoints in your code._
- [Python debugger commands](https://docs.python.org/3/library/pdb.html?highlight=debugger#debugger-commands)
- [pdb++](https://github.com/pdbpp/pdbpp) _This is pdb with some additional nice features like syntax highlighting. To use it, you can `pipenv install --dev pdbpp` and it will automatically be used instead of the built-in pdb._

### Foreign Keys

- [Django Model Field Reference: ForeignKey](https://docs.djangoproject.com/en/4.0/ref/models/fields/#foreignkey)
- [Django Model Field Reference: ManytoMany](https://docs.djangoproject.com/en/4.0/ref/models/fields/#manytomanyfield)
- [Django ORM Cookbook: How to include a Self-Referencing ForeignKey in a Model](https://books.agiliq.com/projects/django-orm-cookbook/en/latest/self_fk.html#how-to-include-a-self-referencing-foreignkey-in-a-model)

### Models & Queries

- [Retrieving Objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#retrieving-objects) You should know how to:
    - retrieve all objects with `all()`
    - retrieve one object with `get()`
    - retrieve specific objects with `filter()`
- [Video: How Model Queries Work in Django](https://www.youtube.com/watch?v=WimXjp0ryOo)
- [Lookups that span relationships](https://docs.djangoproject.com/en/4.0/topics/db/queries/#lookups-that-span-relationships)
- [Field Lookups](https://docs.djangoproject.com/en/4.0/topics/db/queries/#field-lookups)
- [Complex Lookups with Q objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#complex-lookups-with-q-objects) _If you want to include an OR in your search, you will need a Q object._

### Implementing Search

- [LearnDjango: SearchTutorial](https://learndjango.com/tutorials/django-search-tutorial) _Will uses class-based views in this post but you can still follow almost all of his steps and use function-based views._
- [MDN: Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data#the_method_attribute) _The section on the `GET` method shows how to include form data as query parameters._
- [User Interaction with Forms in Django](https://www.mattlayman.com/understand-django/user-interaction-forms) _This reviews content we have already covered about Django forms and also talks about forms from the client side._
- [Django Docs: HttpRequest objects](https://docs.djangoproject.com/en/4.0/ref/request-response/#httprequest-objects) _Documentation about how to get query parameters from a GET request (and other request attributes, including how to access uploaded files)._

## 🦉 Code

- [Django Music example](https://github.com/Momentum-Team-11/example-django-music)
