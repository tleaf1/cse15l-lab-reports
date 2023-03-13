# Lab Report 5

## Exploration of the 'ls' Command

**Overview:** The `ls` command is used to view a list of files or other sub-directories that are in the current working directory. ([Source](https://www.atatus.com/blog/ls-command-in-linux-with-example/))

1) Using the `ls -R` command.

By using the `ls -R` command, we are able to view all the files that exist in the subdirectories of the current directory we are working in. This is useful because instead of going into each directory to find a file we are looking for we can quickly view all subdirectories to find the correct one.

<img width="602" alt="Screen Shot 2023-03-13 at 3 39 27 PM" src="https://user-images.githubusercontent.com/122562580/224848316-43627602-f43f-4b70-b48e-0282f1d2e0b6.png">

In this example we are able to use the `grep` command in conjunction with the `ls -R` command to quickly view the files we might need. Instead of changing directories and then listing them all out again we are able to increase our speed and quickly obtain what we need without even changing directories!

<img width="609" alt="Screen Shot 2023-03-13 at 3 42 07 PM" src="https://user-images.githubusercontent.com/122562580/224848757-c7d6c1f7-ca83-4ea6-9a11-395fdc25cafb.png">

Source(s) used for the `ls -R` command: https://www.hostinger.com/tutorials/linux-commands

2) Using the `ls -lh` command.

Here, we are able to view the files that exist within our current working directory as well as the size of the files. This is useful and important because if storage space is ever an issue we can see if we can remove any files to free up space.

<img width="607" alt="Screen Shot 2023-03-13 at 3 46 59 PM" src="https://user-images.githubusercontent.com/122562580/224849465-f053e70d-faaa-4c0a-9220-79f87a2ef073.png">

Along with this, this command also gives us the time and date that different files were created. This is useful because if we wanted to offload different files after a certain amount of time as well as a certain size we could use this command to see how long ago the file(s) were created. 

<img width="571" alt="Screen Shot 2023-03-13 at 3 54 23 PM" src="https://user-images.githubusercontent.com/122562580/224850433-1af76216-6f20-41d7-8b76-348176873a49.png">

Source(s) used for the `ls -lh` command: https://www.hostinger.com/tutorials/linux-commands

3) Using the `ls -t` command.

By using the `ls -t` command, we are able to view files in the order of when they were created. This is useful because if someone had poor naming conventions when making files we would be able to see them in the order of their creation. This can greatly assist in troubleshooting issues.

<img width="641" alt="Screen Shot 2023-03-13 at 3 59 37 PM" src="https://user-images.githubusercontent.com/122562580/224851231-2d58f472-f0a2-438c-89da-e3d27fd35a58.png">

Here, we can also use this command in order to see which files are more up to date. for instance if three files contain similar info but one is more updated, the `ls -t` command can show us which file has the most recent change. 

<img width="675" alt="Screen Shot 2023-03-13 at 4 07 02 PM" src="https://user-images.githubusercontent.com/122562580/224852007-ac7b3cfb-f767-44fa-b95f-55652f27a6e3.png">

Source(s) used for the `ls -t` command: https://www.atatus.com/blog/ls-command-in-linux-with-example/

4) Using the `ls -p` command.

This command allows the user to see which elements in the output of ls are directories. This is useful because instead of looking one by one at different files, we can immediately see if a file is a directory or not.

<img width="653" alt="Screen Shot 2023-03-13 at 4 14 51 PM" src="https://user-images.githubusercontent.com/122562580/224852902-4fa4cebd-aef9-4c4e-84bd-3ca39d825e85.png">

Here, we can see that there are a mix of files and by uing the `ls -p` command we can quickly identify which ones are directories. This can help us in troubleshooting as well as debugging because sometimes we might mistakenly try to access a file and be unaware that it is a directory. By using this command, we can ease the burden when dealing with many different types of files or very nested directories.

<img width="724" alt="Screen Shot 2023-03-13 at 4 18 13 PM" src="https://user-images.githubusercontent.com/122562580/224853319-5e3aad0c-3051-4487-8ae6-17ddf3130bd7.png">

Source(s) used for the `ls -p` command: https://www.atatus.com/blog/ls-command-in-linux-with-example/
