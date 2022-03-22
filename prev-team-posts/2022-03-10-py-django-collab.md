---
layout: post
title: Collaborating on a web application
tags: phase-2 django collaboration
---

## 🗓️ Today's Topics

- FreeShelf retrospective
- Collaboration in a shared repo

## 🎯 Project: Django Team Project

Today we'll begin our first real team project, with a shared repo. This will require more planning, a lot of communication and coordination, and adding on some new Git skills that will let us collaborate effectively.

You will work in a shared repo and **submit one application** that your team will build together. You need to discuss who will do what, but keep in mind that the work needs to be **shared as equally as possible**.

You have two options to choose from for this assignment. Your team should meet to discuss and **decide today** which one you will do.

Then, the very next thing you should do is determine what **models** you will need and what attributes and relationships they should have. An ER diagram can be very helpful here.

This assignment is due next Thursday at the end of the Phase.

### Dev Teams

For this project, **the first team member listed should accept the assignment** and enter the name of your team.

After that step, the other team members can then accept the assignment and join their team.

- ⚡ **Team ThunderClan**: Alex, K.E., Ryan
- 🏞 **Team RiverClan**: Tyler, Joey, Adam
- 🌬️ **Team WindClan**: Kalen, Emily
- 🕶 **Team ShadowClan**:  Paul, Jocelyn
- 🌠 **Team SkyClan**: Brittany, Osama, Ted

If you want to know where these names came from, [have I got a website for you](https://warriorcats.com/clans-cats/clans).

👉 [**Link to Django Duplex assignment**](https://classroom.github.com/a/dxeLMHQC)

### ✅ Project Checklist

- Set up a new Django project from scratch. There is no starter code in the assignment repo.
- Make sure to create a `.gitignore` file to exclude certain files (like your `.env` file and `db.sqlite3`) from Git. You can get one specific to a Django project at [gitignore.io](https://www.toptal.com/developers/gitignore). Just search for `Django` and copy and paste the text you find there into your `.gitignore` file. It should be placed at the root of your repo.
- Make sure to create a custom user model, following best practices. **Do this before you run any migrations.** [This guide may be helpful to you.](https://learndjango.com/tutorials/django-custom-user-model)
- You may want to install `django-debug-toolbar`, `django-extensions`, and `django-environ`, as we have done in previous projects.

## 🔖 Resources

### Collaboration

- [GitHub Collaboration Docs](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests)
- [Git Collaboration slides](https://slides.com/amy_nc/git-collaboration/)
- [Git in VS Code](https://code.visualstudio.com/docs/introvideos/versioncontrol) _Not everyone loves using git on the command line like I do.  A lot of folks like using the integration in VS Code, so you might want to give it a try. This is a good place to start, but there are many other extensions that you could use as well._
- [Pair Programming Guide](https://tuple.app/pair-programming-guide/template) _This template for a pairing session is practical and actionable, and it can work if there are three of you as well! There are other resources on this site also worth a look._

### Django

- 🍕 [Tips for Using Django's Many-to-Many Field](https://www.revsys.com/tidbits/tips-using-djangos-manytomanyfield/) _This was included in earliers posts too. It's probably the best written explanation of M2M relationships out there, so don't miss it._
- [Django Docs: Related Objects Reference](https://docs.djangoproject.com/en/3.0/ref/models/relations/) _Working with objects that are related to each other via O2M or M2M relationships_
- [Django Docs: Making Queries](https://docs.djangoproject.com/en/3.2/topics/db/queries/) _Queries are what you need to look things up in the database_
- [Creating Interactive Views in Django](https://hackersandslackers.com/creating-django-views/) _Detailed post really breaking down views._
- [Django Slug Tutorial](https://learndjango.com/tutorials/django-slug-tutorial)
- [Django Docs: Built-in Template Tags and Filters](https://docs.djangoproject.com/en/3.0/ref/templates/builtins/)
- [makeareadme.com](https://www.makeareadme.com/) _Guidance for creating your own README file_
- [A great example of a README and a cool project 🏒](https://github.com/minter/tesla_puck)
- [CRC model](http://agilemodeling.com/artifacts/crcModel.htm) _The Class-Responsibility-Collaborator model helps you to reason about how to design your models and relationships._

## 🦉 Code & Notes

- [Django Music App](https://github.com/Momentum-Team-11/example-django-music)
- [Git Collaboration Slides](https://slides.com/amy_nc/git-collaboration)
