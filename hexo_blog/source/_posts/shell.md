---
title: shell
date: 2017-03-30 21:51:05
tags:
---


For most Linux, Unix, and Mac shells.
## Symbolic links
`ln -s target symboliclink`. The target has to exist already.

## Shortcuts
Edit on command line, all with ctrl key

    a / e: move to beginning / end of line
    b / f: move back / forward one character
    k / u: delete all right / left of cursor
    w: delete word left of cursor (same as alt+backspace)
    y: undo above deletions
    l: clear screen

## Using history

    !!: repeat last command
    r / s: search backward / forwards through history.
    ctrl + p / n: same as up arrow / down arrow respectively, step through history
    a space before a command omits it from history

## Navigating directories

`pwd`: print working director, i.e. the directory where you are
`cd` or `cd ~`: change to home directory. `~` (called tilde) is a shortcut for your home directory. `cd ~/Library` cds to `/Users/[current user]/Library`.
`cd -` : cd to previous directory
`tree`: display an "ASCII art" tree representation of the directory structure. Not installed by default on all operating systems. Can be installed with `yum install tree`, `sudo apt-get install tree`, `brew install tree`, etc.
## Users and permissions

`chmod -options filename`: lets you change the read, write, and execute permissions on your files
Reading directories and files
`ls`: lists  files. Useful switches include `-l` (more info) `-a` (hidden files) `-rt` (sort ascending by time).
`stat`: display info about file on disk
`touch`: create or update a file
`less`: opens the file in a vi-like environment
`cat`: print contents of file. tac prints in reverse order
`head`: print first 10 lines of file
`tail`: print last 10 lines of file
`diff`: compare two files
`wc`: display number of lines, words and characters in a file
`grep`: search a file
## Environment

    export: display all environment variables
    echo $SHELL: display shell in use
    echo $BASH_VERSION  # displays bash version

## Job control

    j / m: same as Enter
    ctrl+c: kill current command
    z: suspend command, resume with fg in the foreground, or bg in the background
    pstree: display running processes in a dependency tree

## Users and permissions

    id: print user and group id

## Misc. and somewhat useless

    cal: display a calendar for the current month
    yes [somestring]: prints a string until an interrupt (e.g. ctrl+c) is detected
    rev: enters interactive mode and reverses any input string
