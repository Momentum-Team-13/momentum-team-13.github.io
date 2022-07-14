---
layout: post
title: 🐻 Queries & Using the Shell 🐻
tags: phase-3 back-end queries shell
---

## Today's Topics

- Interacting with models in the shell
- Queries and more queries

## 🎯 Project: Still Working on Habit Tracker

Habit Tracker is **due on Monday**. You can do this! 💪 **What do you need to figure out in order to finish it?**

### 📖 Read | 📺 Watch | 🎧 Listen

- [Database Design for Beginners](https://youtu.be/1VsSXRPEBo0) _This is a talk from RailsConf, which is focused on Ruby on Rails (Rails is a framework for building web applications in Ruby, very similiar to Django). The talk is an excellent introduction to how to think about your data model -- that is, the logic that drives the decisions you make about the models in your code and the structure of your database. Please watch it all the way through; even though it uses Ruby examples you should be able to get the gist._

This rest of this section is material to prep for the topic we will begin next week: building APIs.

- [RESTful APIs](https://restful-api-design.readthedocs.io/en/latest/intro.html) Read up through the "Standard Methods" subsection of the section on "Methods". You can read more if you want to but it gets pretty deep.
- [Safia Abdullah, You and Me Learn All About HTTP](https://dev.to/captainsafia/you-and-me-learn-all-about-http-with-safia-abdalla-3nd0)
- [Web APIs Explained By Selling Goods From Your Farm](https://blog.codeanalogies.com/2018/02/27/web-apis-explained-by-selling-goods-from-your-farm/)


## 🔖 Resources

### Using the shell (Django's interactive REPL, not pipenv shell)

- [Official Django docs on using the shell](https://docs.djangoproject.com/en/4.0/ref/django-admin/#shell)
- [Django extensions: `shell_plus`](https://django-extensions.readthedocs.io/en/latest/shell_plus.html?highlight=shell_plus#shell-plus)

#### 🦄 PRO TIPS

- `django-debug-toolbar` has a SQL panel that will show you the queries you are running in the view.
- With `shell_plus`, you can see output of all the SQL queries if you run it like this:

```py
python manage.py shell_plus --print-sql
 ```

### Lookups

- [Pretty Printed Video: How Model Queries Work in Django](https://youtu.be/WimXjp0ryOo)
- [Pretty Printed Video: Querying One-to-Many Relationships in Django](https://youtu.be/iwNBwG8RBok )
- [Django QuerySets](https://docs.djangoproject.com/en/4.0/topics/db/queries/#retrieving-objects)
- [Django Model Managers](https://docs.djangoproject.com/en/4.0/topics/db/managers)
- [Django Queries: Retrieving Objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#retrieving-objects)
- [Field lookups](https://docs.djangoproject.com/en/4.0/topics/db/queries/#field-lookups)
- [Lookups that span relationships](https://docs.djangoproject.com/en/4.0/topics/db/queries/#lookups-that-span-relationships)
- [Lookups with Related objects](https://docs.djangoproject.com/en/4.0/topics/db/queries/#related-objects)
- [Django Related Objects Reference](https://docs.djangoproject.com/en/4.0/ref/models/relations/#related-objects-reference)
- [Complex lookups with Q](https://docs.djangoproject.com/en/4.0/topics/db/queries/#complex-lookups-with-q-objects)
- [F objects](https://docs.djangoproject.com/en/4.0/ref/models/expressions/#django.db.models.F)

### Constraints

- [Django Docs: model constraints](https://docs.djangoproject.com/en/4.0/ref/models/options/#constraints) -> this gives you the general format/syntax
- [Django Docs: UniqueConstraint](https://docs.djangoproject.com/en/4.0/ref/models/constraints/#uniqueconstraint)

### Aggregate & Annotate

- [PrettyPrinted Video: Basics of Django Aggregations](https://youtu.be/2MFAV-arSuI)
- [Pretty Printed Video: How to Use Annotate in Django](https://youtu.be/KbwmdKl-QbI)
- [Django docs:Aggregate & Annotate](https://docs.djangoproject.com/en/4.0/topics/db/aggregation/)
- [Django docs: Combining Aggregations with other QuerySets](https://docs.djangoproject.com/en/4.0/topics/db/aggregation/#s-aggregations-and-other-queryset-clauses)
- [Aggregation Functions](https://docs.djangoproject.com/en/4.0/ref/models/querysets/#aggregation-functions) (e.g., `Avg`, `Count`, `Min`, `Max`)

### 🦉 Code & Notes

- [Django Model Queries CheatSheet](https://github.com/Momentum-Team-13/notes/blob/main/django-queries.md)
- [Django Recipes App](https://github.com/Momentum-Team-13/example-django-recipes)
