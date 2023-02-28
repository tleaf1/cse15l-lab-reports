# Lab Report 4

## Competition Task Walkthrough

**Step 1: Logging in to ieng6**

Keys pressed: `<Ctrl>-R`, typed 'ssh', `<space>`, `<enter>` 

The command `ssh cs15lwi23apz@ieng6.ucsd.edu` was already in the bash search history so I was able to directly access it with the Ctrl-R command. Also since I successfully set up my ssh key, I was able to successfully log in without entering my password.

  <img width="510" alt="Screen Shot 2023-02-27 at 4 53 56 PM" src="https://user-images.githubusercontent.com/122562580/221724084-763398f9-d81f-4367-a969-a4434ef30e43.png">

  
**Step 2: Cloning the Repository for the Task**
  
Keys pressed: `<Ctrl> - R`, typed 'git', `<space>`, typed 'c', `<enter>`. 

Since the `git clone git@github.com:tleaf1/lab7.git` command was already in the search history I was able to directly access it as well and use the command without repeatedly using the up arrow command or typing the full command out.

  <img width="547" alt="Screen Shot 2023-02-27 at 4 59 09 PM" src="https://user-images.githubusercontent.com/122562580/221724763-0a0985bd-6e3d-43b9-9557-2b2945edefcc.png">

  
**Step 3: Initial Run of JUnit Tests**

Keys pressed: Typed 'cd lab7', `Ctrl` + R, then I typed 'javac' and then `enter`, then `Ctrl` + R, then I typed 'java' then `space` and then `enter`.

Similar to the last two commands, the commands to run JUnit were already in the bash history so I was able to quickly run them again by using the Ctrl-R command without having to go and copy paste the two commands or remember how to type them all out.

<img width="825" alt="Screen Shot 2023-02-27 at 5 03 59 PM" src="https://user-images.githubusercontent.com/122562580/221725456-dc99ebea-e01f-41ef-a5af-bb11521739ae.png">

  
**Step 4: Editing the Java File to Fix the Error**
  
Keys pressed: I typed 'nano +43 Li' `<tab>` then typed '.java', `<enter>`, `<right>` x12, `<backspace>`, typed '2', `<Ctrl-O>`,`<enter>`, `<Ctrl-X>`. 

By adding '+43' to my command I was able to have nano open up directly to where the error was in the code, making it easier to quickly make necessary changes so that the tests can successfully pass. Along with this, pressing `<tab>` autofilled the name of the java file without having to type the full name out.

<img width="840" alt="Screen Shot 2023-02-27 at 5 08 58 PM" src="https://user-images.githubusercontent.com/122562580/221726140-963f89d8-5ebd-4333-8b64-25a6ec7ac16e.png">

**Step 5: Rerunning the Tests**

Keys pressed: `<up><up><up><up><enter>`,`<up><up><up><up><enter>`. 

Since these commands were recently ran, I used the up arrow to quickley access them instead of using the 'Ctrl-R' command that was previously used. the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was four up in the command history and after it was ran, the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` command was then four up in the command history.

<img width="836" alt="Screen Shot 2023-02-27 at 5 14 17 PM" src="https://user-images.githubusercontent.com/122562580/221726934-7757de55-da25-433e-a6e0-40eb5b9ed00f.png">

**Step 6: Committing and Pushing to GitHub!**

Keys pressed: `<Ctrl-R>`, then I typed 'git a', `<enter>`; `<Ctrl-R>`, then I typed 'git co', `<enter>`; `<Ctrl-R>`, then I typed 'git p', `<enter>`. 

Since these three commands ('git add ListExamples.java', 'git commit -m "updated"', and 'git push', respectively) were already in the bash command history I used the 'Ctrl-R' command again to make their execution much quicker.

<img width="834" alt="Screen Shot 2023-02-27 at 5 17 27 PM" src="https://user-images.githubusercontent.com/122562580/221727742-814b8904-bfce-458e-bdfa-bb2b631465da.png">

