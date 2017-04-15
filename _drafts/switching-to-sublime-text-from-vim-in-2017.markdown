---
layout: post
title: Switching to Sublime Text from Vim in 2017
---

## Background

I am a freelance software developer.  I mostly work on Ruby on Rails and Ember.js projects.  Prior to this week, I would work almost exclusively in the terminal with terminal Vim and tmux.  I still use tmux and [tmuxinator](https://github.com/tmuxinator/tmuxinator) to set up the dev environment for the current project I am working on (changing to the correct directory, switching to the correct ruby version, starting servers, etc.).  I am not scared of the terminal and continue to use it for Git, the Rails console, running tests, among other things.

## Why I am leaving Vim

I have been using Vim for over 4 years.  I am not the best Vim user, but I know it enough that any other editor that forces me to use the mouse would make me less productive.  I have slowly written a `.vimrc` that fits my needs and use many plugins.  I really liked that I could use it in the terminal where I could easily switch to do other things on the terminal.

What I didn't like about Vim was that it a good number of plugins always felt like a hack.  Vim has built-in functionality to be extended, but every plugin seemed to make gradually slower, more than on other editors.

One example is CtrlP.  It is currently the most recommended way of switching files in Vim.  The default setup can be improved by using [The Silver Searcher](https://github.com/ggreer/the_silver_searcher) to find the files and using [ctrl-py-matcher](https://github.com/FelikZ/ctrlp-py-matcher) to match files with your search query.  I _always_ had issues with it.  From having to refresh every time I made a new file to folders such as `node_modules` being included in the results unless I refreshed again (although this could be an issue with The Silver Searcher).  I have tried for a long time to get it to work as well as it works on editors such as Atom and Sublime Text, but it's something I could never achieve.

Another popular plugin is Syntastic.  I absolutely hate the way it displays the errors.  It is not a smooth transition from "no error" to "error".  Not much to say here, it just looks awful, yet it is highly recommended.

I don't use many plugins, most of them are just to work with newer languages such as Rust and Elixir.  For all other plugins, you need to really consider whether you need it or not.  If you don't stick to the bare essentials, it is likely that Vim will start to slowdown.

Also, very few people actually use Vim to its potential.  "With Vim you never have to use a keyboard" is not a good argument.  Any popular editor usually has a "Vim mode" that you can install.  If you want to convince someone to specifically use the actual editor Vim, mention something else.

## Why Sublime Text