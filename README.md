# How to get a new classroom site up and running

## jekyll.rb

Jekyll is a ruby + markdown static site generator that we use to create a simple blog-style content site for our classes.

### Setup

You will need Ruby installed and the ability to install Ruby gems with bundler.

You might like using [`rbenv` to install Ruby versions](https://github.com/rbenv/rbenv).

Follow the QuickStart docs from Jekyll to install `jekyll` and `bundler`.

Once you have cloned the repo you can start [setting up a new team](#config-for-a-new-team).

### File structure

To publish a post you'll need to create a new md doc in `_posts/`. Filenames are important and should follow this structure:

```
2021-10-19-js-ajax.md
```

You can copy draft posts from the previous team to use as a basis for your posts. Jekyll won't compile posts in a `_drafts` folder, so you might want to create one locally; it's gitignored.


## Config for a new team

There are several places where you will need to edit files for the current team's number. In this template those places are indicated with an `X`, like `Momentum Team X` or `momentum-team-x`.

You'll also want to create a new GitHub pages repo in the team's GitHub organization. The repo should be named `momentum-team-x.github.io` and configured to deploy to GitHub pages using the `main` branch.

### _config.yml

This file is used by jekyll to configure the site. Make sure you change the relevant data for the current team.




