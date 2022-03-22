---
layout: post
title: 🍔 Django with a Side of JavaScript 🍟
tags: phase-2 django javascript ajax search
---

## 🗓️ Today's Topics

- Progress report on Code Snippets and Flashcards
- Incorporating JavaScript in a Django application

## 🎯 Project: Code Snippets | Flashcards

Still working on your project. (っ^з^)♪♬

### Where you should be with **Flashcards** today

#### These tasks should be pretty much done

A logged in user should be able to...

- see a list of all the decks
- see the cards in a given deck (after it is selected from the list, for instance)
- see the question on a given card with no answer showing
- create a new deck via a web form
- create new cards and associate them with a deck

#### You might still be working on

- A user can run through the deck one card at a time
- A user can click to reveal the answer on a card
- A user can mark a card as answered correctly or incorrectly
- You should be able to record that data somewhere. If decks belong to one user and are not shared, then you could record this on your deck, but it's up to you how you model this.
- You have some way to show a user how they did at the end of the deck
- Bugs
- Styling and README

### Where you should be with **Code Snippets** today

#### These tasks should be pretty much done

A logged in user should be able to...

- see a list of all public snippets
- see a list of their own snippets
- create new snippets from scratch
- edit and delete existing snippets

#### You might still be working on

- A user can search snippets
- A user can copy someone else's snippet
- Syntax highlighting for snippets displayed to the user
- Bugs
- Styling and README

## 🔖 Resources

### Debugging while you work

Setting a `breakpoint()` can help you figure out what code you need in your views. You can also use the Django shell to test your queries.

- [Django Debug Toolbar docs](https://django-debug-toolbar.readthedocs.io/en/latest/)
- [RealPython Debugging with Pdb](https://realpython.com/python-debugging-pdb/) _The built-in Python debugger (Pdb) lets you set breakpoints in your code._
- [Python debugger commands](https://docs.python.org/3/library/pdb.html?highlight=debugger#debugger-commands)
- [pdb++](https://github.com/pdbpp/pdbpp) _This is pdb with some additional nice features like syntax highlighting. To use it, you can `pipenv install --dev pdbpp` and it will automatically be used instead of the built-in pdb._

### JavaScript & Django

- [Django and AJAX](https://realpython.com/django-and-ajax-form-submissions/)
- [Fetching Data with Ajax and Django](https://www.brennantymrak.com/articles/fetching-data-with-ajax-and-djang`o.html) -> This article is really helpful and has really good code examples. Important notes:
  > By including the 'X-Requested-With' header set to 'XMLHttpRequest' [in the AJAX request], the view will be able to check if the request is AJAX or not.

{% highlight python %}
    # In the view function that handles the AJAX request you need to check this condition:
    request.headers.get('x-requested-with') == 'XMLHttpRequest'
{% endhighlight %}

- [Django docs on the above](https://docs.djangoproject.com/en/4.0/ref/request-response/#django.http.HttpRequest.is_ajax)
- [Working with AJAX in Django](https://testdriven.io/blog/django-ajax-xhr/)
- [MDN: Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) _Remember JS?_ 🥴 _Here's a refresher on using Fetch._
- [Django CSRF with AJAX](https://docs.djangoproject.com/en/4.0/ref/csrf/#ajax)
- [LearnDjango: Static Files and Templates](https://learndjango.com/tutorials/django-static-files)

### ⭐ EXTRA/TMI

- [Django Views the Right Way](https://spookylukey.github.io/django-views-the-right-way/the-pattern.html) _This is a detailed, informative deep dive on function-based views in Django_
- [jQuery](https://jquery.com/) _This is not something I recommend using right now, but I include it here because a lot of the resources about using JavaScript in a web browser refer to it (several of the articles above do). It is not as popular as it once was, and it is incompatible with a framework like React. But you will sometimes come across it, and you may end up working with it at your job, so you might as well recognize it when you see it and look it up if you ever need to use it._
- [Understanding the CSRF threat and protection measures](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)

## 🦉 Code

- [Django Music example](https://github.com/Momentum-Team-11/example-django-music)
