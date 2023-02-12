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

**2) using the grep **

