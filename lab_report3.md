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

Unlike the grep -v command used previously, grep -w will return results that contain the entire string that was inputted. Here, instead of filtering out results containing the string Athens, we are returning all results that contain the string Athens.
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

**3) Using the grep -c command**

Using this command we are able to return a count for the amount of files containing the specified query as well as how many times it appears. Below are some of the results using the keyword "Tiana". Note that only the files containing the query have a count above zero.
```
$ grep -c "Tiana" berlitz2/*
berlitz2/Algarve-History.txt:0
berlitz2/Algarve-Intro.txt:0
berlitz2/Algarve-WhatToDo.txt:0
berlitz2/Algarve-WhereToGo.txt:0
berlitz2/Amsterdam-History.txt:0
berlitz2/Amsterdam-Intro.txt:0
berlitz2/Amsterdam-WhatToDo.txt:0
berlitz2/Amsterdam-WhereToGo.txt:0
berlitz2/Athens-History.txt:0
berlitz2/Athens-Intro.txt:0
berlitz2/Athens-WhatToDo.txt:0
berlitz2/Athens-WhereToGo.txt:0
berlitz2/Bahamas-History.txt:0
berlitz2/Bahamas-Intro.txt:0
berlitz2/Bahamas-WhatToDo.txt:0
berlitz2/Bahamas-WhereToGo.txt:0
berlitz2/Bali-History.txt:0
berlitz2/Bali-WhatToDo.txt:0
berlitz2/Bali-WhereToGo.txt:0
berlitz2/Barcelona-History.txt:0
berlitz2/Barcelona-WhatToDo.txt:0
berlitz2/Barcelona-WhereToGo.txt:0
berlitz2/Beijing-History.txt:6
berlitz2/Beijing-WhatToDo.txt:1
berlitz2/Beijing-WhereToGo.txt:18
```
Here, we can use the grep -c command to see how many directories contain the specified query. This is useful because instead of listing all directories and counting each one individually, we are able to see a quick result with only one command!
```
$ ls | grep -c berlitz
2
```
Source(s) for the grep -c command: I used the command man grep on my machine as well as [this](https://qpeng.org/computer/grep.htm) useful website.

**4) Using the grep -n command**

Here we are using grep -n in order to display how many files contain the tring "Athens" as well as which specific line they are on. This is useful because instead of just returning the names of the files we can see which specific line they are on in order to make our search faster.
```
$ ls | grep -n Athens
9:Athens-History.txt
10:Athens-Intro.txt
11:Athens-WhatToDo.txt
12:Athens-WhereToGo.txt
```
Along with this, the grep -n command can also help us to find line(s) in a text file that contain specific words. Note that I did not include the entirety of the command result as I wanted to highlight the fact that the -n command will include line number of the specified query.
```
$ grep -n "Lucayans" berlitz2/*
berlitz2/Bahamas-History.txt:6
berlitz2/Bahamas-History.txt:7
```

