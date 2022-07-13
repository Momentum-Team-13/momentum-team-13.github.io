---
title: "Python Code Break: list comprehensions and formatting output"
layout: default
nav_exclude: true
---

## Working with list comprehensions and formatting output

### exercise 1

Write a [list comprehension](https://docs.python.org/3/tutorial/datastructures.html?highlight=comprehension#list-comprehensions) that takes each word in a list of words and puts it in all caps.

```py
phrases = ["everything is fine", "have a seat", "holy cow"]
# your list comprehension should produce a list that looks like this:
# ['EVERYTHING IS FINE', 'HAVE A SEAT', 'HOLY COW']
```

Remember that the basic structure of a list comprehension is:

```py
new_list = [<expression> for <each_item> in <a_list>]
```
### exercise 2

Rewrite a `remove_from_list function` to use a list comprehension to remove the item.

The `remove_from_list` function should take a list of items and an item to remove from that list, and return a new list that contains everything from the original list except for that item. It should remove every occurrence of the item in the list (if it appears more than once).

### exercise 3

Write a function `print_freq_results(results)`. This function should take an argument `results` that is a list of tuples like the following:

 ```py
 [
     ('her', 33),
     ('all', 12),
     ('which', 12),
     ('she', 7),
     ('their', 7),
 ]
 ```

 This function should print (not return) output like the following:

 ```sh
   her | 33 *********************************
   all | 12 ************
 which | 12 ************
   she | 7  *******
 their | 7  *******
 ```

😎 HINT: You're going to need some [string methods](https://docs.python.org/3/library/stdtypes.html#string-methods) to align the characters.
