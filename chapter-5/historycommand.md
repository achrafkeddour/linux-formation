Using ! in Linux Command History

The ! operator in Linux allows you to quickly re-execute commands from the command history without manually retyping them. Here's how to use it effectively:


---

1. Re-run a Command by History Number

Each command in the history list is assigned a number.

Use !<number> to execute a specific command based on its history number.
Example:

sysadmin@localhost:~$ history
    1  date
    2  ls
    3  cal 5 2030
sysadmin@localhost:~$ !3
cal 5 2030



---

2. Re-run the Most Recent Command

Use !! to execute the last command you ran.
Example:

sysadmin@localhost:~$ date
Wed Dec 12 04:32:36 UTC 2018
sysadmin@localhost:~$ !!
date
Wed Dec 12 04:32:38 UTC 2018



---

3. Re-run the Most Recent Command Matching a Name

Use !<command-name> to re-execute the most recent occurrence of a specific command in the history.
Example:

sysadmin@localhost:~$ ls
Desktop Documents Downloads
sysadmin@localhost:~$ cd ..
sysadmin@localhost:~$ !ls
ls
Desktop Documents Downloads



---

4. Re-run a Command from the Bottom of History

Use !-<number> to execute a command relative to the end of the history list (e.g., !-2 runs the second-to-last command).
Example:

sysadmin@localhost:~$ history
    5  date
    6  ls
    7  history
sysadmin@localhost:~$ !-2
ls



---

5. Run and Edit a Command

After recalling a command using !, you can edit it before executing by positioning the cursor with the arrow keys.


6. Avoiding Repetitive Typing

Using ! is especially helpful for automating repetitive tasks or debugging, saving significant time when working with long commands.

