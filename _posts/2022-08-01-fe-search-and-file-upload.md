---
layout: post
title: 🦊 Search and File Uploads 🦊
tags: phase-3 phase-3-fe
---

## 🗓️ Today's Topics

- Implementing search in your application 🔍
- Image & file uploads: forms and requests

## Example Search Request with Query Params

Remember the [iTunes API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/Searching.html#//apple_ref/doc/uid/TP40017632-CH5-SW1)? To get search results, you needed to include query params that specified the search fields and terms you wanted to use.

Here's how you might make a request that uses query params using [axios](https://github.com/axios/axios#request-config). (Note: this example depends on `searchTerm` and `token` being defined in your code.)

```js
axios.get('https://drf-library-api.herokuapp.com/api/books',
  {
    params: {search: searchTerm},
    headers: {Authorization: `Token ${token}` }
  }
)
```

### A note on search in React

You could also perform a search without making an AJAX request, by filtering data that you already have in React. Here are a couple of examples of how you could do that.

- [Create a search bar from scratch](https://blog.logrocket.com/create-search-bar-react-from-scratch/)
- [How to Build a Search Bar in React](https://www.emgoto.com/react-search-bar/)

## Example Request to Upload a File

This is an update to an existing record; notice that we are using the PATCH verb. In this case you are including the file itself as the body of the request; notice that the file is in the second position as an argument to `axios.patch()` as the body of the request. We are also setting specific headers required by the server to handle the binary file attachment, in addition to the Authorization header.

```js
axios.patch(url, file, {
  headers: {
    Authorization: 'Token ' + token,
    'Content-Type': file.type,
    'Content-Disposition': `attachment; filename=${file.name}`
  }
}).then(res => console.log(res.data))
```

NOTE: If you Google how to include a file attachment in an ajax request, you'll see a lot of references to using the FormData object. You can do it that way, but you don't have to; the above method will work just fine as long as you know how to access the file that is being uploaded by the user. If you _do_ want to use FormData, please discuss with your back end devs, as they will need to make sure that they can parse that content.

Here's info about [using FormData objects](https://developer.mozilla.org/en-US/docs/Web/API/FormData/Using_FormData_Objects) if you want to know more about that.

See the resources below for more information about using a file input element and accessing a selected file. The `useRef()` hook will be helpful to get the files from the input element after a user has selected a file using the form.

## 🔖 Resources

- [Generate random images from Unsplash without an API](https://awik.io/generate-random-images-unsplash-without-using-api/)
- [Uncontrolled components](https://reactjs.org/docs/uncontrolled-components.html)
- [Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html) - class-based component examples
- [useRef hook](https://reactjs.org/docs/hooks-reference.html#useref)
- [MDN: File input type](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file)
- [MDN: Accessing selected files](https://developer.mozilla.org/en-US/docs/Web/API/File/Using_files_from_web_applications#accessing_selected_files)
- [Custom hook recipes](https://usehooks.com/)
- [More custom hooks](https://github.com/streamich/react-use)
- [Official React docs on custom hooks](https://reactjs.org/docs/hooks-custom.html)
