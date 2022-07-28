---
layout: post
title: 🐻 File Upload with Django and DRF 🐻
tags: phase-3 phase-3-be full-text-search deploy file-upload
---

## 🗓️ Today's Topics

- How are the projects coming along? 👀
- Letting users upload files/images using AWS S3

## 🎯 Project

Keep on going. 💪 🚀

Today let's get you past any blockers you may be experiencing and talk through next steps.

By now you should have provided your front end with a way to log in and log out, and endpoints to see at least some data. You can create some data via the Django admin so that you can see your GET requests working. By tomorrow you should be able to create (at least some)resources via POST requests.

## 📖 Read | 📺 Watch | 🎧 Listen

### File Upload

- [Django File (and Image) Uploads Tutorial](https://learndjango.com/tutorials/django-file-and-image-uploads-tutorial) -> A good and very recent post from Will Vincent; he does not include all the necessary info to make file uploads work in production but otherwise it's a good overview.
- 📖 [File Upload with DRF](https://goodcode.io/articles/django-rest-framework-file-upload/)
- 🎧 + 📖 [Success with Static Files](https://www.mattlayman.com/django-riffs/success-static-files/)
- 📖 [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) -> Skim this -- this is Amazon's documentation and it gets really in-depth.
    - 📺 [Introduction to S3](https://www.youtube.com/watch?v=77lMCiiMilo) -> Also from Amazon

### Search

On Monday we'll be covering full-text search in your API, but if you have time you can check these resources out in advance.

- [Search from the Ground Up](https://www.youtube.com/watch?v=is3R8d420D4&list=PL2NFhrDSOxgXXUMIGOs8lNe2B-f4pXOX-&index=2) -> DjangoCon 2019 video explaining search in detail
- 📖 [Basic and Full-Text Search with Django and Postgres](https://testdriven.io/blog/django-search/)
- 📖 [Blog post with more on full-text search](https://www.netlandish.com/blog/2020/06/22/full-text-search-django-postgresql/)
- 📖 [If you want A LOT more detail about full-text search in Postgres and Django, this blog piece has you covered](https://pganalyze.com/blog/full-text-search-django-postgres)

## 🔖 Resources

### File uploads

- [Django Docs: ImageField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#imagefield)
- [Django Docs: FileField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#filefield)
- [Pillow: Python Imaging Library](https://pillow.readthedocs.io/en/stable/)
    - [`django-imagekit`](https://django-imagekit.readthedocs.io/en/latest/) -> If you want to resize images when they are uploaded, or do any kind of image processing, you will need this. Don't add it unless you know you need it.
- [How to Set Up Amazon S3](https://simpleisbetterthancomplex.com/tutorial/2017/08/01/how-to-setup-amazon-s3-in-a-django-project.html)
    - [AWS S3 Free Tier Info](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=categories%23storage)
- [`django-storages`](https://django-storages.readthedocs.io/en/latest/index.html)
- [DRF `FileUploadParser`](https://www.django-rest-framework.org/api-guide/parsers/#fileuploadparser)

#### A request with a file attachment using Insomnia

- Select the right HTTP method for your endpoint.
- Choose binary file attachment from the JSON menu (where you normally put the body of a request)
- Set headers on the Headers tab (this example assumes an image file in jpeg format, named `profile-photo.jpg`):

  ```txt
  Content-Type: image/jpeg
  Content-Disposition: attachment; filename=profile-photo.jpg
  ```

For more information on the values for `Content-Type`:

- [MDN Content-Type Header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Type)
- [MDN MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

#### CORS for file upload

Assuming you are using `django-cors-headers`, you'll need to add the following to `settings.py` to allow the request headers necessary for file attachments:

```py
# in settings.py

from corsheaders.defaults import default_headers

CORS_ALLOW_HEADERS = list(default_headers) + [
    'content-disposition',
]
```

### Authentication

Make sure you are sharing the Djoser information with your front end. You should include the authentication endpoints in your API documentation or project README.

- [Base Endpoint Guide for Djoser](https://djoser.readthedocs.io/en/latest/base_endpoints.html) -> includes create a new user and other nice stuff
- [Token Authentication Endpoint Guide for Djoser](https://djoser.readthedocs.io/en/latest/token_endpoints.html) -> details on the token auth endpoints

### Creating a properly hashed password

In order to save a properly hashed password when you create a new user in the Django Admin, make sure you are using `UserAdmin` in `admin.py` so that you have that option in the admin interface. If you don't do this and save an unhashed password, you will run into authentication errors.

```py
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin
...
admin.site.register(User, UserAdmin)
```

You can also change a password from the command line:

- [Django Docs: Changing a password](https://docs.djangoproject.com/en/4.0/topics/auth/default/#changing-passwords)

## 👾 Code

- [DRF Library API](https://github.com/Momentum-Team-13/example-drf-library)
