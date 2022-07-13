---
title: Python Code Break 3
layout: default
nav_exclude: true
---

## Working with lists

### exercise 1

Write a function called `remove_from_list` that takes a list of items and an item to remove from that list: ``remove_from_list(list_of_items, item_to_remove)``

The function should return a new list with the item removed. Write code to test your function, like the following:

```py
remove_from_list(['Dallas', 'Kelly', 'Courtney', 'Hayden', 'Chase'], 'Hayden')
# should return  ['Dallas', 'Kelly', 'Courtney', 'Chase']
```

Make sure your function removes all instances of the item. Write code to test this.

```py
remove_from_list(['MI', 'AK', 'SC', 'AK', 'DE'], 'AK')
# should return `['MI', 'SC', 'DE']
```

### exercise 2

Write a function `remove_many_from_list(list_of_items, items_to_remove)` that takes two lists, a list of items, and a list of items to remove from that original list. You can re-use `remove_from_list` or write it from scratch.

```py
ingredients = ['onions',
               'habanero hot sauce',
               'tomatoes',
               'tortillas',
               'corn',
               'black beans',
               'avocados',
               'cheese',]
foods_my_kids_hate = ['habanero hot sauce', 'avocados']

remove_many_from_list(ingredients, foods_my_kids_hate)
# should return ['onions', 'tomatoes', 'tortillas', 'corn', 'black beans', 'cheese']
```
