---
title: Switching to Sublime Text from Vim in 2017
---

## Background

I am a freelance software developer.  I mostly work on Ruby on Rails and Ember.js projects.  Prior to this week, I would work almost exclusively in the terminal with NeoVim (_never_ a GUI Vim) and tmux.  I still use tmux and [tmuxinator](https://github.com/tmuxinator/tmuxinator) to set up the dev environment for the current project I am working on (changing to the correct directory, switching to the correct ruby version, starting servers, etc.).  I am not scared of the terminal and continue to use it for Git, the Rails console, running tests, among other things.

## Why I am leaving Vim

I have been using Vim for over 4 years.  I am not the best Vim user, but I know it enough that any editor that forces me to use the mouse would make me less productive.  I have slowly written a `.vimrc` that fits my needs and use a few plugins.  I really liked that I could use it in the terminal where I could easily switch to do other things on the terminal.

What I didn't like about Vim was that a good number of plugins always felt like a hack.  Vim has built-in functionality to be extended, but every plugin seemed to make it gradually slower, more than on other editors.

One example is CtrlP.  It is currently the most recommended way of opening files in Vim.  The default setup can be improved by using [The Silver Searcher](https://github.com/ggreer/the_silver_searcher) to find the files and using [ctrl-py-matcher](https://github.com/FelikZ/ctrlp-py-matcher) to match files with your search query.  I _always_ had issues with it.  From having to refresh every time I made a new file, to folders such as `node_modules` being included in the results unless I refreshed again (although this could be an issue with The Silver Searcher).  I have tried for a long time to get it to work as well as it works on Sublime Text, but I was never able to get it even _close_ to the performance and quality of the results of Sublime Text.

Another popular plugin is Syntastic.  I absolutely hate the way it displays the errors.  It is not a smooth transition from "no error" to "error".  Not much to say here, it just looks awful, yet it is highly recommended.

I don't use many plugins, most of them are just to work with newer languages such as Rust and Elixir.  For all other plugins, you need to really consider whether you need it or not.  If you don't stick to the bare essentials, it is likely that Vim will start to slowdown.

One of the settings that really slowed my Vim down, was the `relativenumber` setting.  If you are not familiar with this setting, what it does is instead of displaying the actual line numbers in the file, it displays the how many lines away a line is relative to your current line.  If that sounds confusing, just type `:set relativenumber` and you will see what I mean.  Apparently this can make your Vim really slow when moving up and down.  I had this setting for years and it never ocurred to me that this could be affecting my Vim speed.  It was only through some random web browsing that I found out that this made Vim much slower.

Other parts of Vim I just never really understood.  Swap files have always annoyed me and I would disable them.  When I would edit a file, Vim wouldn't automatically reload it without me doing it manually (and only realizing I need to do this after editing a file).  In order to automaticall reload files you need to add a line or two in your `.vimrc` to look for watch for file changes then reload.  It's not a simple one line setting.  I never tried it because I was worried about slowing down the editor.

Also, very few people actually use Vim to its potential.  "With Vim you never have to use a mouse" is not a good argument.  Any popular editor usually has a "Vim mode" that you can install and you can achieve native Vim productivity.  If you want to convince someone to specifically use the actual editor Vim, being mouseless is not going to work if they can already emulate Vim commands in their editor.

And probably the most superficial and shallow reason I switched: I want prettier font rendering.  I didn't spend money on a retina Macbook Pro to be limited to 256 colors.

## Why Sublime Text

My issues with Vim were small, but still very annoying.  I wanted to find an editor that was just as fast but wouldn't slow down to a crawl once I started modifying it to my needs.  So I went back to Sublime Text which I haven't used since 2012.  Back then, Vintage mode (the name for the "Vim" mode in Sublime Text) had a few missing commands that I regularly used in Vim.  Now those commands are available in Sublime Text so I am not missing out on anything from switching away from Vim, at least for my workflow.  It's also **much** easier to extend than Vim and does not slow down as much when customized.  Sublime Text just feels faster and smoother for me than Vim ever did.  If I had added all the Vim plugins needed to match Sublime Text's functionality, it would have been even slower.

I admit it, I never paid for Sublime Text when I was using it.  So I decided to pay for it this time and support the project.  Now, I know some of you will say: "But Atom and Visual Studio Code are free and open source!"  I don't give a damn.  Open source is an awesome thing.  However, open source, with its potential to bring hundreds (if not thousands) of developers together to help create amazing software, has given us: editors that run slower than [what we had available in the 90s](https://en.wikipedia.org/wiki/Gedit).  More and more "desktop" software will be built like this.  I'd rather do my part to ensure good desktop software will continue to exist, even if it's proprietary.  I will not use shitty software just because it's open source.

Also, why not Emacs?  I wanted to change my editor, not my operating system :P.

## You should still learn how to use Vim

I hope I have not discouraged you to not learn how to use Vim.  Everything I have learned in using Vim has carried over to Sublime Text.  Almost every popular editor and IDE has a Vim plugin.  Being forced to use only the keyboard in an editor has made me more productive.  Also, if you will be ssh'ing into servers frequently, the best editor available is usually Vi or Vim.
