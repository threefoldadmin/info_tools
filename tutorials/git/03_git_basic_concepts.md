# GIT Basic Concepts

## Introduction

Git is a source code version control system that has become a de-facto standard in the engineering world. It allows many people collaborate on the same source code.

Why it is so cool and why people like it?
It allows to achieve several goals:

* Many people can work simultaneously on the same set of documents
* Have multiple branches of work in progress by different people
* Have current 'active' or most correct finalized set of documents available to everyone
* Save every single change in the history and easily track and navigate over the history of the changes.

It is a little techy but since you learn it you will love it.

In this manual we will cover only very basics needed for several most common operations with it. It can do much more and if you want to learn more, there are extensive manuals availbe in google :)

## Concepts and definitions

* Repository (or repo) - a place where all documents and their history is stored. Git is a distributed system. There is origin (main) repo on a remote server accessible to everyone and local repo that you use for your daily work. Local and remote repo are synced by Push and Pull actions
* Pull - the act of taking most recent changes from remote repo to local repo (my machine)
* Push - the act of submitting most recent changes from local repo to remote repo
* Clone - the act of making a new copy of remote repo locally (when you start your work with new repo)
* Staging - the act when you ask your local GIT to take a look (index)  on files that you worked with locally
* Commit - When you take all staged changes and put it into local repo
* Changeset (or Version) - batch of files changed at the same time and recorded in a repo as a result of a commit
* Branch - history of changes in GIT can be visualized as a tree, where you can make a branch of the repo if you need to make a big alternative changes and you are not sure yet if they should appear for everyone as a main version
* Merge - the process of merging conflicting changes between your local changes and remote changes or between different branches

These are the definitions and actions you should understand for basic work.
If you want to learn in-depth, you can find on internet huge amount of manuals and articles on any aspect of GIT.
