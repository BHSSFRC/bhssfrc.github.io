Using `git`
---

* auto-gen TOC:
{:toc}

## This document is not...
the `git` manual. This document only covers how we structure the repository branches. If you have no idea what `git` is and how to use it, there are a plethora of finely made cheatsheets online. For example:

* [GitHub's cheat sheet.](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf) Despite it suggesting you install thier `git` GUI, you should still avoid it like the plauge.
* [The DuckDuckGo cheat sheet.](https://duckduckgo.com/?q=git+cheat+sheet&t=ffab&ia=cheatsheet)

## General branch structure in one image
[![git flow diagram](https://raw.githubusercontent.com/arslanbilal/git-cheat-sheet/master/Img/git-flow-commands-without-flow.png)](https://raw.githubusercontent.com/arslanbilal/git-cheat-sheet/master/Img/git-flow-commands-without-flow.png)

(Click the image to expand it)

## A saner explanation
Ever heard of the term "git flow"? If you know what that refers to, odds are you may skip reading this.

Git allows for "dividing" a repository into **branches** of **commits.** In git flow, two main branches exist: `master` and `develop`.

* `master` is the "main" branch of the repository. It is the version you recieved when you initially cloned the repository from GitHub.
* `develop` is the "mad science practically ready to release" branch. It contains all the features slated for release/merging into `master`. 

Both branches should contain running, working as expected code. (`develop` is allowed signifigant leeway in the "working as expected" department.)
