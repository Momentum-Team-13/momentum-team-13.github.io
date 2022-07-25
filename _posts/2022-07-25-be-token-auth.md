---
layout: post
title: 🐻 Token Authentication and CORS 🐻
tags: phase-3 phase-3-be djoser token-auth cors
---

## Today's Topics

- Token authentication in DRF with Djoser
- CORS headers

## 🎯 Collaborative Project

Work with your team. Tonight, plan out your **models** -- please draw a diagram! -- and write down **a list of the endpoints** you think you will need. It should take you some time to talk this through. What data will those endpoints have to return? Will your endpoints need to accept any data (remember you can do this in the body of the request or using part of the URL)?

Your list of planned endpoints should look something like (this is a _partial_ list using examples from Habit Tracker. You're going to need a bunch more endpoints than this). Keep in mind that you should include endpoints ONLY if you need them, so consider the actions that you need to support according to the project requirements.

_Example planning for endpoints (you'll need more than these, of course):_

| **Request URL**             |   	| **Description**                                            	|
|:---------------------------	| ---	|:------------------------------------------------------------	|
| `GET api/habits`          	|   	| returns a list of all habits for the logged in user        	|
| `GET api/habits/<int:pk>` 	|   	| returns details about one habit and its associated records 	|
| `POST api/habits`         	|   	| create a new habit                                         	|

**No writing code yet**! Today should be used for planning only. We'll cover working together on GitHub tomorrow.

## 📖 Read | 📺 Watch | 🎧 Listen

- [Finally Understand Auth in DRF - a Will Vincent talk](https://www.youtube.com/watch?v=pY-oje5b5Qk) -> Will isn't using the Djoser library but he does a great job of reviewing different auth strategies and why you would choose one or the other. Watch this for a better understanding and overview of authentication.
- [Julia Evans comic explaining CORS better than MDN does](https://twitter.com/b0rk/status/1162392625057583104?lang=en)
- [More Julia Evans on the Same Origin Policy](https://twitter.com/b0rk/status/1155493682885341184)
- [Simple Is Better Than Complex: How to Implement Token Authentication in DRF](https://simpleisbetterthancomplex.com/tutorial/2018/11/22/how-to-implement-token-authentication-using-django-rest-framework.html) _This does NOT use Djoser, but it's a great walkthrough of some of what Djoser does for you if you would like more detail._

## 🔖 Resources

### Authentication

- [Djoser documentation](https://djoser.readthedocs.io/en/latest/)
- [DRF docs: Token-based authentication](https://www.django-rest-framework.org/api-guide/authentication/#tokenauthentication)
- [The Ultimate Tutorial for Django REST Framework: Login and Authentication](https://sunscrapers.com/blog/django-rest-framework-login-and-authentication/) _This uses the Djoser library._

### CORS

- [MDN CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
    - [MDN Access-Control-Allow-Origin Header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin)
- [Django CORS Guide](https://www.stackhawk.com/blog/django-cors-guide/)
- [`django-cors-headers`](https://github.com/adamchainz/django-cors-headers)

### Permissions

- [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
- [Pro-Tip: Logical operators with DRF Permissions](https://www.revsys.com/tidbits/tip-about-drf-permissions/)
