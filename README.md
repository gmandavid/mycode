Lab Objective
These labs will guide you through hands-on, step-by-step exercises, with detailed explanations for each step.

The virtual environment you will use to perform these labs is available to you 24/7 throughout the duration of your course. We do not turn them off in between sessions.

Getting Started
Let's make sure you are ready to start running through these labs.

Even so, you may have to use a new key-combination to use the copy-paste functionality. Let's practice it now.

If you click on the little clipboard icon  in a lab, it will copy whatever text or code block is next to it, and will be available to paste into the virtual machine.

student@bchd:~$ # copy me!

After clicking on the , you will then be able to paste the command or code block wherever you would like.

Typically, you will want to paste into the Virtual Machine's terminal.

Each browser is different, but there are several ways to do this:

In the terminal, right click, then select paste (or) paste as plain-text (depending on the browser)
Shift Insert
Ctrl Shift v
Go ahead and try to paste the text of # copy me! into your terminal now.

Fundamental Commands
Not every person in this course has experience using a terminal to interact with a computer. This section is for those who may not have previous experience using a Linux terminal.

First of all, take a look at your command prompt to try to understand what it can teach us. It should look like:

student@bchd:~$

student is the name of the user
bchd is the hostname of the machine
~ (to the right of the colon) shows us the present working directory. Specifically, ~ refers to this user's home directory of /home/student.
$ shows us that this is a typical user (vs. # would indicate that it is the root user)
Now let's run some fundamental commands to get to know our environment a little bit better. Remember, we are starting in our /home/student directory for this.

pwd - [present working directory] shows you what directory you are in.

student@bchd:~$ pwd

/home/student
ls - list out the contents of the current directory.

student@bchd:~$ ls

static
cd - [change directory] - allows you to move to a different directory. Here we can move to the static directory.

student@bchd:~$ cd static

mkdir - [make directory] - allows you to make a new directory. Let's make one called training.

student@bchd:~/static$ mkdir training

Also, let's make sure we can see that we made this training directory.

student@bchd:~/static$ ls

training
And let's move into the training directory.

student@bchd:~/static$ cd training

touch - makes a blank file.

student@bchd:~/static/training$ touch example_01.txt

Verify that the file named example_01.txt is there now.

student@bchd:~/static/training$ ls

example_01.txt
echo - returns text to the standard output.

student@bchd:~/static/training$ echo Alta3 Research Training rocks!

Alta3 Research Training rocks!
The > character allows us to redirect standard output to a different place, normally a file.

student@bchd:~/static/training$ echo Alta3 Research has AWESOME labs! > myfile.txt

The >> characters allow us to redirect standard output and append it to the end of a file.

student@bchd:~/static/training$ echo Alta3 Research has AMAZING labs! >> myfile.txt

cat - [concatenate] prints file(s) to standard output.

student@bchd:~/static/training$ cat myfile.txt

Alta3 Research has AWESOME labs!
Alta3 Research has AMAZING labs!
mv - [move] allows us to move a file or directory (often used to rename files).

student@bchd:~/static/training$ mv myfile.txt ego_fuel.txt

Verify that the file has moved.

student@bchd:~/static/training$ ls

ego_fuel.txt example_01.txt
Make sure that the contents of the file have not changed.

student@bchd:~/static/training$ cat ego_fuel.txt

Alta3 Research has AWESOME labs!
Alta3 Research has AMAZING labs!
history - shows all of the commands performed in this shell session.

student@bchd:~/static/training$ history

    1  # copy me
    2  pwd
    3  ls
    4  cd static
    5  mkdir training
    6  ls
    7  cd training
    8  touch example_01.txt
    9  ls
   10  echo Alta3 Research Training rocks!
   11  echo Alta3 Research has AWESOME labs! > myfile.txt
   12  echo Alta3 Research has AMAZING labs! >> myfile.txt
   13  cat myfile.txt
   14  mv myfile.txt ego_fuel.txt
   15  ls
   16  cat ego_fuel.txt
   17  history
man - [manual] show the manual pages (aka documentation) for a given command. This is helpful for understanding any commands you may not feel comfortable with.

student@bchd:~/static/training$ man ls

To quit out of this view, press the keyboard key q

Excellent work! Now, let's move back to the home directory before you start working on the next lab.

student@bchd:~/static/training$ cd ~

Your prompt should now be back to: student@bchd:~$

If you have any questions throughout the course, please feel free to reach out to:

Your Instructor
Email the Alta3 Research's Support Team support@alta3.com
Helpful Resources
Alta3 Research Instruction & Training
Alta3 Research Posters & Cheat Sheets
Alta3 Research YouTube

Common Questions and Solutions
My screen has "dots" around it :(
If you have more than one screen open, the "smallest" resolution wins. Therefore, the solution is to close the second tab you have open.
I typed exit too many times and my CLI session closed!
Press the Refresh icon on your browser to refresh your session and create a new tmux session
How do I get my content out of the tmux (CLI) environment?
The "best" way is probably by using git and GitHub. Alternatively, if you move content into the ~/static/ folder, you may access it by changing the "source" of your right-most pane in the split-screen session. To change the source, click on the icon that looks like three sheets of paper in the upper-right hand corner.
Will the lab environments "shut off" this week?
No. The your lab environment is on 24x7, until the termination date.
Can I close the tab to live.alta3.com
Yes! Unless you clear your internet cache, you should just be able to revisit your custom course link to regain access. If you are asked to log-in again, simply use the same email address and handle to regain access.
