---
layout: post
title: "Git text adventure"
date: 2013-02-28 13:43
comments: true
categories: 
---

At the [PDX Git Together](pdxgit.com) last night, [Lyzi Diamond](https://twitter.com/lyzidiamond) and many others expressed their frustration at Git, but in very constructive ways.  People called for better, friendlier tutorials.

Git is hard, and if anyone tells you otherwise they're lying.

Git is hard, and its not your fault if you don't get it.

[Eric Willhelm](https://twitter.com/ericsbrain) had one of his usual brain waves, what if Git were a text adventure game?

[What if it were](https://github.com/schwern/git-adventure)?  Here's how it might look...

<!-- more -->

Welcome to The World of Git!
----------------------------

Git is a version control system of frustration, danger and low cunning!

You're in an empty directory, there is no repository here.
Its dark and you are likely to be eaten by a troll.<br />
`git> status`

*A disembodied voice booms!*
    fatal: Not a git repository (or any of the parent directories): .git
There is no git repository here!  You must *init* one first to continue your quest.<br />
`git> init`

*A disembodied voice booms!*
    Initialized empty Git repository in /Dungeons/git/player/.git/
You create a new repository!  Huzzah!

The [.git directory](http://gitready.com/advanced/2009/03/23/whats-inside-your-git-directory.html) springs into existence on the floor before you.  Its warm glow lights the room and keeps the trolls at bay.  Everything you do with git will be contained in this one directory.

A clear pool of water appears at your feet.  It is known by many names in many tongues: the index, the cache, the [staging area](http://gitready.com/beginner/2009/01/18/the-staging-area.html).  We will refer to it here as the staging pool.  Before anything is added to the repository it must pass through the staging pool.  When you *add* to the repository you are saving a copy in the staging pool.

A new label appears at the start of the repository, it says "master".  It is your current branch.  It will move with you while you *commit* more things in the repository.

You are on a branch called "master" in the initial commit to your repository.  The repository is empty.  The staging pool is empty, it seems to want you to *add* something.

You take a file called README from your backpack and place it in the directory.  You must *add* this file to the staging area.

There is an untracked file here called "README".<br />
`git> add`

*A disembodied voice booms!*
    Nothing specified, nothing added.
The Git Lords are trying to tell you that you must say which files you want to *add*.  In this case its the README file.<br />
`git> add README`

You dip the README into the staging area.  Its reflection appears in the water.  As you put the README back on the floor you notice the reflection of the README remains.  The staging area has remembered a copy of README.

You are on a branch called "master" in the initial commit to your repository.  The repository is empty.  The staging pool contains a copy of the README file.  You must get the contents of the staging pool into the master branch.  The repository seems to want you to *commit* to it. <br />
`git>`
