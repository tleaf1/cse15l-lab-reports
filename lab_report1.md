# Lab Report 1
## Successfully accessing a remote server

**Step 1: Installing Visual Studio Code**

In order to install VSCode on your device, go to [the VSCode website](https://code.visualstudio.com/) and
follow the instructions for your correct operating system (MacOS, Windows, etc.).

Once you have VSCode downloaded, navigate to where you downloaded it and follow the steps to
install it on to your computer.

Once you have successfully installed VSCode, it should look something like this: 

<img width="1021" alt="VSCode Screen" src="https://user-images.githubusercontent.com/122562580/212164216-fec20d9e-e9f6-4432-a166-2b284f19f217.png">

**Step 2: Remotely Connecting to a Server**

In order to remotely connect into a server, go into Visual Studio Code and click Terminal -> New Terminal. An
image of what this looks like is below.
<img width="1022" alt="Screen Shot 2023-01-12 at 11 47 13 AM" src="https://user-images.githubusercontent.com/122562580/212166284-f357b08f-2251-4640-a4f4-bc0f4f7d6169.png">

Once you have done this you will now ssh into the server. In order to do this, type the command `ssh cs15lwi23zz@ieng6.ucsd.edu` into 
your console. **Remember**: you must replace the 'zz' in the command with the letters from your course specific account.

If this is your first time accessing this server you will receive a prompt asking if you would like to continue. Type
`yes` and then press enter. 

You should see something like this:
<img width="897" alt="Screen Shot 2023-01-12 at 5 47 26 PM" src="https://user-images.githubusercontent.com/122562580/212218331-9cbf9fd4-b801-4529-8510-62e5a6cfa8ce.png">


Next, you will be prompted to enter your password. Please enter the password associated with your account. If your password does not work, please use [this tutorial](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit) to reset your password.

Congratulations! You have now successfully accessed a remote server!
You terminal should now look something like this:
<img width="644" alt="Screen Shot 2023-01-13 at 12 23 36 PM" src="https://user-images.githubusercontent.com/122562580/212412603-ed89dea3-8b31-4fe5-9d1a-a67965263eec.png">


**Step 3: Testing Out Commands**

Now we will begin using some basic commands to navigate and understand this server.

To begin, try putting `pwd` into your terminal to view your current working directory and to see where you are currently at in the server. Next, type the command `ls` to list the items that are in the current directory.

Your screen should look something like this:

<img width="520" alt="Screen Shot 2023-01-13 at 12 41 34 PM" src="https://user-images.githubusercontent.com/122562580/212415424-01787b17-704d-48ce-8610-a39bc57c5b45.png">


Nice! You are now successfully navigating a remote server via the command line. If you wish to exit the terminal you can use the keyboard shortcut `Ctrl + D` or you can type in the command `exit`.

For your own practice, here are some other commands you can use to explore this server:
