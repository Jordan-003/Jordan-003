## Lab 02

- Name: Jordan Cox
- Email: cox.389@wright.edu

## Part 1 Answers

1. Command & steps to create an SSH key pair: ssh-keygen -t ed25519 --> choose file name --> enter password
2. Steps to add public key to GitHub profile: cd .ssh --> cat (.pub file) --> (copy line) --> settings in github --> SSH and GPG keys --> New SSH key --> add title and paste in key box
3. git command to clone repository: git clone git@github.com:Jordan-003/Jordan-003.git

## Part 2 Answers

The answers for this section are to help you record what steps  
are needed to create a file locally (in your cloned repo)  
and push them (sync) with GitHub.  Only `git` commands are 
valid answers

1. git command to view the status of the repository: git status
2. git command example to add a file for tracking: git add file
3. git command to commit changes: git commit -m "changes"
4. git command to sync local commits with GitHub: git push
5. git command to sync commits on GitHub to `clone`d repository: git pull

## Part 3 Answers

1. `chmod u+r bubbles.txt`
    - Means: For bubbles.txt, the user is now allowed to read the file.
2. `chmod u=rw,g-w,o-x banana.cabana`
    - Means: For banana.cabana, the user can read and write in the file, the group can no longer write in the file, others can no longer execute the file.
3. `chmod a=w snow.md`
    - Means: For snow.md, the user, group, and others can write in the file.
4. `chmod 751 program`
    - Means: For program, the user can read, write, and execute, the group can write and execute, and others can only execute.
5. `chmod -R ug+w share`
    - Means: For share, the user and group can now write in all files.

## Part 4 Answers

1. Command to create new user: sudo adduser jcox
2. Path to user's home directory: /home/jcox
3. Evaluate if `ubuntu` can add files to user's home directory: No. Ubuntu cannot get into the directory
4. Command to switch to user: su jcox
5. Command(s) to go to user's home directory: cd /home
6. Evaluate if user can add files to user's home directory: No, they cannot. sudo touch file --> touch: cannot touch 'file': Permission denied
7. Command to switch to `ubuntu`: exit
8. Command to return to `ubuntu` home directory: cd /home

## Part 5 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`: sudo addgroup crew
2. Command(s) to add `ubuntu` & user to group `crew`: sudo adduser ubuntu crew, sudo adduser jcox crew
3. Command to modify `share` to have group ownership of `crew`: sudo chgrp crew share
4. Command to switch to user: su jcox
5. Command to add file to `share`: sudo touch filename
6. Evaluate why these steps allowed the above action: Users ubuntu and jcox were added into crew. Crew gained ownership of share which meant that ubuntu and jcox gained ownership.

## Part 6 Answers

For each, write the command used or answer the question posed.

1. Command to create file using `sudo`: sudo touch sudowho.txt
2. Evaluate (in plain text) the permission of the file: ubuntu can make changes in the file with sudo. Others can only read.
3. Provide a method to edit the file without modifying permissions: sudo vim sudowho.txt
4. Command(s) to modify permissions: sudo chown ubuntu sudowho.txt
