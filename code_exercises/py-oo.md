---
title: "Python Code Break: OO"
layout: default
nav_exclude: true
---

## Define a User class and create user objects

### Step 0

Create a new Python file and name it whatever you want. This is where you will write the code that follows.

### Step 1

Make a class named `User`. Add the following attributes to your class (in the `__init__()` method):

- `name`
- `email`
- `city`
- `state`

Create two different user instances using your class and save them to variables (something like `user1` and `user2`).

When you run your file, print out f-strings that display info using attributes from each user instance:

```txt
Anton lives in Durham, NC.
Cecil lives in San Francisco, CA.
```

### Step 2

Add a `__str__` method to your class that displays the identity and attributes of an instance when it is printed.

#### step 2 example

Say you have a `Game` class; the `__str__` method could look like this (although there are lots of other options!):

```python
def __str__(self):
    return f"<Game score={self.score} tries={self.tries}>"
```

If you print a game instance with that `__str__()` method (for example, `print(game1)`), the output should look like this:

```python
<Game score=0 tries=8>
```

### Step 3

Make a method named `location` that returns a string listing the user's city and state (e.g., "Durham, NC").

### Step 4

Add an attribute called `is_active` to your class. This attribute should have a default value of `True`.

Then, make another method called `deactivate` that changes the value of the `is_active` attribute to `False`.

Create an instance of a user and test that it works. Try resetting the attribute to `True` using the assignment operator and checking the value again.

### Step 5

Add an attribute called `login_count` that keeps a count of how many days in a row a user logs in. Its default value should be 0.

Add a method called `increment_login_count` that adds 1 to the `login_count` attribute each time it is called and returns the updated count.

Then add a method called `reset_login_count` that resets the count to 0.

Create an instance of a user and test that this works.
