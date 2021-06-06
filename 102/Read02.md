# GIT


## What is The GIT ?

Local VCS (Version Control System)system that allows you to revisit various versions of a file or set of files by recording changes. Through version control,
one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes.

## What is The need of The GIT ?

The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS).
This system entails a single server storing all changes and file versions, which can be accessed by various clients.

## Local Operations

Git mostly relies on local operations because most necessary information can be found in local resources.This allows for process expediency because 
a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work 
on a project even when not online or on a VPN.

##Tracking Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of
information in transit.

## Setting up a Git Repository

Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init
Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.

To start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”


### Git Website

You can download Git by visiting this link and following the posted directions [GIT](http://git-scm.com/download/win) 

