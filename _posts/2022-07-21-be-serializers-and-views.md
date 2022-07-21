---
layout: post
title: 🐻 Views and Serializers in DRF 🐻
tags: phase-3 phase-3-be django rest
---

## 🗓️ Today's Topics

- Views and viewsets
- Nesting and customizing serializers
- Permissions

## 🎯 Project

Keep on with your API building 😎 💪! What do you need to know to get it working?

By now you should have a **list of endpoints** that your API offers, even if they are not all complete yet. A good place for this would be in your README, formatted with Markdown. This list should show the URLs along with the HTTP methods/verbs, and ideally should include an example of the JSON that has to be included in the request body (for any requests that send data in the body) and an example of the JSON response that will be returned, for each endpoint. **This list will be helpful for your own testing and it can serve as necessary documentation for your API.**

Here is an example of what your documentation might look like for an endpoint to create a book:

___

#### Create a new book

**request**

_Requires authentication._

`title` and `author` are required fields.

```json
POST api/books

{
   "title": "The Anatomy of Melancholy",
   "author": "Robert Burton",
   "publication_year": 1621
}
```

**response**

```json
201 Created

{
  "pk": 6,
  "title": "The Anatomy of Melancholy",
  "author": "Robert Burton",
  "publication_year": 1621,
  "featured": false,
  "reviews": []
}

```

___

By today or tomorrow, your app should respond with json to GET requests for all habits/books, for one habit/book, and for one book/habit's associated objects (daily records for habits; reviews or trackers for books). By tomorrow you should also have at least some of your POSTs working, and can begin working on updates and deletes.

💁 **Make sure you test your endpoints in Insomnia** to confirm that they are working as intended. Use `show_urls` from django-extensions to help you check what urls you have defined.

**Is your app deployed to Heroku yet?** 👀 🚀

## 🔖 Resources

- [Django REST Framework Docs](https://www.django-rest-framework.org/)
- [Article on DRF Generic Views](https://testdriven.io/blog/drf-views-part-2/)
- [Classy DRF](https://www.cdrf.co/)

### Serializers

- [Using Different Read and Write Serializers in DRF](https://www.revsys.com/tidbits/using-different-read-and-write-serializers-django-rest-framework/)
- [How to Save Extra Data to a DRF Serializer](https://simpleisbetterthancomplex.com/tutorial/2019/04/07/how-to-save-extra-data-to-a-django-rest-framework-serializer.html) - _for example, when you need to associate a user with an object that you are creating._
- [Effectively using DRF Serializers](https://testdriven.io/blog/drf-serializers/)

### Permissions

- [DRF Permissions](https://testdriven.io/blog/drf-permissions/)
- [Built-in Permission Classes in DRF](https://testdriven.io/blog/built-in-permission-classes-drf/)
- [Custom Permissions in DRF](https://testdriven.io/blog/custom-permission-classes-drf/)
- [Pro Tip about DRF Permissions](https://www.revsys.com/tidbits/tip-about-drf-permissions/) _This shows how to combine permissions with logical operators like `and` and `or`_

## 👾 Code

- [Example Recipes API](https://github.com/Momentum-Team-13/example-django-recipes)
