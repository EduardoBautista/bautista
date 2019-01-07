---
title: Automatically correct typos in Git
date: '2016-01-24 20:33:00'
tags:
- git
- tips
---

## TL;DR
`git config --global help.autoCorrect -1`

## The Details
Ah yes.  Once again you have typed `git stauts` and have received the infamous response:

```
git: 'stauts' is not a git command. See 'git --help'.

Did you mean this?
	status
```

Never fear, you can configure git to automatically correct your typos using the `help.autoCorrect` configuration option.  Here is the description in the documentation:

>Automatically correct and execute mistyped commands after waiting for the given number of deciseconds (0.1 sec). If more than one command can be deduced from the entered text, nothing will be executed. If the value of this option is negative, the corrected command will be executed immediately. If the value is 0 - the command will be just shown but not executed. This is the default.

So basically, you use it like this:

`git config [--global | --local | --system ] help.autoCorrect [number of deciseconds (0.1 sec) to wait before executing or a negative number for to execute immediately]`

Here is how I use it:

`git config --global help.autoCorrect -1`

Now you will get this message:

>WARNING: You called a Git command named 'stauts', which does not exist.
>Continuing under the assumption that you meant 'status'

**Edit**: I updated the "TL;DR" command to run immediately instead of waiting 0.1 seconds.
