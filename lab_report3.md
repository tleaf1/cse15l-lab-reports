# Lab Report 3

## The 'grep' Command

**1) Using the 'grep -v' command**

Here, we are using the grep -v command to filter out non-fiction from our results when we use the ls command. This is useful because it can narrow our search for specific files without having to sift through multiple directories.
  ```
  $ ls | grep -v non-fiction
  travel_guides
  ```

In this example, we are usign grep -v in order to see only berlitz1. This is useful because there are two directories that contain the string berlitz but by using grep -v we can differentiate between directories that we do not want to show up or use.
  ```
  $ ls | grep -v 2
  berlitz1
  ```
Source(s) for the grep -v command: I used this [wikibooks](https://en.wikibooks.org/wiki/Grep) site to understand the grep -v command

**2) using the grep -w command**

Unlike the grep -v command used previously, grep -w will return results that contain the string that was inputted. Here, instead of filtering out results containing the string Athens, we are returning all results that contain the string Athens.
```
$ ls | grep -w Athens
Athens-History.txt
Athens-Intro.txt
Athens-WhatToDo.txt
Athens-WhereToGo.txt
```
However, in this example nothing is returned because the grep -w command is case sensitive. While it may be annoying, it is useful to ensure that you are returning exactly what you need so that your results are not mixed with items that are not needed.
```
$ ls | grep -w athens
```
Source(s) for the grep -w command: My source for this command can be found [here](https://man7.org/linux/man-pages/man1/grep.1.html).
