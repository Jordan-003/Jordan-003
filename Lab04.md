## Lab 04

- Name: Jordan Cox
- Email: cox.389@wright.edu

## Part 1 - Task Tracker

Verify that `tt` made it to your GitHub repository for this course and is in your `Lab04` folder.  No answers will be written here unless you would like to leave a note to the TAs

## Part 2 - Sample Runs

### User Guide

Fill in with your user guide here

echo "add: add a task to $tasks"
echo "complete: remove a task from $tasks"
echo "view: view the content in $tasks"
echo "clear: remove $tasks"

### Sample runs

Example of using `add` task
```
bash tt add jog
Task added
bash tt add sprint
Task added
```

Example of using `complete` task
```
bash tt complete jog
Task removed
```

Example of using `view` tasks
```
bash tt view
sprint
```

Example of using `clear` tasks
```
bash tt clear
Remove all tasks? [y/n]
(y or Y, n or N)
```

Example of using `help`
```
echo "add: add a task to $tasks"
echo "complete: remove a task from $tasks"
echo "view: view the content in $tasks"
echo "clear: remove $tasks"
```

## Part 5 - PATH for all

- Chosen PATH directory: $HOME/.ssh/Jordan-003/Lab04
- Link preference (hard or symbolic): symbolic
   - Justification of preference for this use case: The link is connected to the content of the file.
- Command to create link: ln -s ~/.ssh/Jordan-003/Lab04/tt soft-link
- Notes about permissions modified: 
- How you tested that you can run `tt` from anywhere on filesystem:
- How you tested that other users can run `tt`:

## Extra Credit

Note here *what* you did to the script for the extra credit and provide additional demonstrations.
