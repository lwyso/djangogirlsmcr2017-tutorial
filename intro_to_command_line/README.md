# Introduction to the command-line interface

> This chapter is covered in [Your new friend: Command Line](https://www.youtube.com/watch?v=jvZLWhkzX-8) video should you wish to watch at a later date.

It's exciting, right?! You'll write your first line of code in just a few minutes! :\)

**Let us introduce you to your first new friend: the command line!**

The following steps will show you how to use the black window all hackers use. It might look a bit scary at first but really it's just a prompt waiting for commands from you.

> **Note** Please note that throughout this book we use the terms 'directory' and 'folder' interchangably but they are one and the same thing.

## What is the command line?

The window, which is usually called the **command line** or **command-line interface**, is a text-based application for viewing, handling, and manipulating files on your computer. Much like Windows Explorer or Finder on Mac, but without the graphical interface. Other names for the command line are: _cmd_, _CLI_, _prompt_, _console_ or _terminal_.

## Open the command-line interface

To start some experiments we need to open our command-line interface first.

<!--sec data-title="Windows" data-id="windows_prompt" data-collapse=true ces-->

Go to Start menu → All Programs → Accessories → Command Prompt.

<!--endsec-->

<!--sec data-title="OS X" data-id="OSX_prompt" data-collapse=true ces-->

### Mac OS X

Applications → Utilities → Terminal.

<!--endsec-->

<!--sec data-title="Linux" data-id="linux_prompt" data-collapse=true ces-->

It's probably under Applications → Accessories → Terminal, but that may depend on your system. If it's not there, just Google it :\)

<!--endsec-->

## Prompt

You now should see a white or black window that is waiting for your commands.

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_prompt" data-collapse=true ces-->

If you're on Mac or Linux, you probably see `$`, just like this:

{% filename %}command-line{% endfilename %}
```
$
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_prompt2" data-collapse=true ces-->

On Windows, it's a `>` sign, like this:

{% filename %}command-line{% endfilename %}
```
>
```
<!--endsec-->

Each command will be prepended by this sign and one space, but you don't have to type it. Your computer will do it for you :\)

> Just a small note: in your case there may be something like `C:\Users\ola>` or `Olas-MacBook-Air:~ ola$` before the prompt sign and that's 100% correct.

The part up to and including the `$` or the `>` is called the _command line prompt_, or _prompt_ for short. It prompts you to input something there.

In the tutorial, when we want you to type in a command, we will include the `$` or `>`, and occasionally more to the left. You can ignore the left part and just type in the command which starts after the prompt.

## Your first command \(YAY!\)

Let's start with something simple. Type this command:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_whoami" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ whoami
```

<!--endsec-->

<!--sec data-title="Windows" data-id="windows_whoami" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> whoami
```

<!--endsec-->

And then hit `enter`. This is our result:

{% filename %}command-line{% endfilename %}
```
$ whoami
olasitarska
```

As you can see, the computer has just printed your username. Neat, huh? :\)

> Try to type each command; do not copy-paste. You'll remember more this way!

## Basics

Each operating system has a slightly different set of commands for the command line, so make sure to follow instructions for your operating system. Let's try this, shall we?

### Current directory

It'd be nice to know where are we now, right? Let's see. Type this command and hit `enter`:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_pwd" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ pwd
/Users/olasitarska
```
> Note: 'pwd' stands for 'print working directory'.

<!--endsec-->

<!--sec data-title="Windows" data-id="windows_cd" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> cd
C:\Users\olasitarska
```
> Note: 'cd' stands for 'current directory'.

<!--endsec-->

You'll probably see something similar on your machine. Once you open the command line you usually start at your user's home directory.

---

### List files and directories

So what's in it? It'd be cool to find out. Let's see:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_ls" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ ls
Applications
Desktop
Downloads
Music
...
```

<!--endsec-->

<!--sec data-title="Windows" data-id="windows_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> dir
 Directory of C:\Users\olasitarska
05/08/2014 07:28 PM <DIR>      Applications
05/08/2014 07:28 PM <DIR>      Desktop
05/08/2014 07:28 PM <DIR>      Downloads
05/08/2014 07:28 PM <DIR>      Music
...
```

<!--endsec-->

---

### Change current directory

Now, let's go to our Desktop directory:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_move_to" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ cd Desktop
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_move_to" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> cd Desktop
```

<!--endsec-->

Check if it's really changed:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_pwd2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ pwd
/Users/olasitarska/Desktop
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_cd2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> cd
C:\Users\olasitarska\Desktop
```

<!--endsec-->

Here it is!
> PRO tip: if you type `cd D` and then hit `tab` on your keyboard, the command line will automatically autofill the rest of the name so you can navigate faster. If there is more than one folder starting with "D", hit the `tab` button twice to get a list of options.

---

### Create directory

How about creating a practice directory on your desktop? You can do it this way:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_mkdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ mkdir practice
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_mkdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> mkdir practice
```

<!--endsec-->

This little command will create a folder with the name `practice` on your desktop. You can check if it's there just by looking on your Desktop or by running a `ls` or `dir` command! Try it. :)

> PRO tip: If you don't want to type the same commands over and over, try pressing the `up arrow` and `down arrow` on your keyboard to cycle through recently used commands.

---

### Exercise!

Small challenge for you: in your newly created `practice` directory create a directory called `test`. (Use `cd` and `mkdir` commands.)

#### Solution:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_test_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ cd practice
$ mkdir test
$ ls
test
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_test_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> cd practice
> mkdir test
> dir
05/08/2014 07:28 PM <DIR>      test
```

<!--endsec-->

Congrats! :\)

---

### Clean up

We don't want to leave a mess, so let's remove everything we did until that point.

First, we need to get back to Desktop:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_back" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ cd ..
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_back" data-collapse=true ces-->


{% filename %}command-line{% endfilename %}
```
> cd ..
```

<!--endsec-->

Using `..` with the `cd` command will change your current directory to the parent directory \(that is, the directory that contains your current directory\).

Check where you are:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_pwd3" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ pwd
/Users/olasitarska/Desktop
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_cd3" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> cd
C:\Users\olasitarska\Desktop
```

<!--endsec-->

Now time to delete the `practice` directory:

> __Attention__: Deleting files using `del`, `rmdir` or `rm` is irrecoverable, meaning _the deleted files will be gone forever_! So be very careful with this command.

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_rm" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ rm -r practice
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_rmdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> rmdir /S practice
practice, Are you sure <Y/N>? Y
```

<!--endsec-->

Done! To be sure it's actually deleted, let's check it:

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_ls2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ ls
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_dir2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
> dir
```

<!--endsec-->

### Exit

That's it for now! You can safely close the command line now. Let's do it the hacker way, alright? :\)

<!--sec data-title="OS X and Linux" data-id="OSX_Linux_exit" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}
```
$ exit
```
<!--endsec-->

<!--sec data-title="Windows" data-id="windows_exit" data-collapse=true ces-->


{% filename %}command-line{% endfilename %}
```
> exit
```

<!--endsec-->

Cool, huh? :\)

## Summary

 Here is a summary of some useful commands:

Command (Windows) | Command (Mac OS / Linux) | Description                | Example
----------------- | ------------------------ | -------------------------- | ---------------------------------------------
exit              | exit                     | close the window           | **exit**
cd                | cd                       | change directory           | **cd test**
cd                | pwd                      | show the current directory | **cd** (Windows) or **pwd** (Mac OS / Linux)
dir               | ls                       | list directories/files     | **dir**
copy              | cp                       | copy file                  | **copy c:\test\test.txt c:\windows\test.txt**
move              | mv                       | move file                  | **move c:\test\test.txt c:\windows\test.txt**
mkdir             | mkdir                    | create a new directory     | **mkdir testdirectory**
rmdir (or del)    | rm                       | delete a file              | **del c:\test\test.txt**
rmdir /S          | rm -r                    | delete a directory         | **rm -r testdirectory**

These are just a very few of the commands you can run in your command line, but you're not going to use anything more than that today.

If you're curious, [ss64.com](http://ss64.com) contains a complete reference of commands for all operating systems.

## Ready?

Let's dive into Python!

