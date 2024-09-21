## Lab 03

- Name: Jordan Cox
- Email: cox.389@wright.edu

## Part 1 Answers

1. `ssh` command before configuring `config` file: ssh -i labsuser.pem ubuntu@34.228.102.218
2. HostName: 34.228.102.218
3. User: ubuntu
4. IdentityFile: ~/.ssh/labsuser.pem
5. `~/.ssh/config` contents: 

```
#ssh -i labsuser.pem ubuntu@34.228.102.218

Host 2350
        HostName 34.228.102.218
        User ubuntu
        IdentityFile ~/.ssh/labsuser.pem
```

6. `ssh` command after configuring an entry in the `config` file: ssh 2350

## Part 2 Answers

1. `printenv HOME > thishouse`
   - Explanation: Creates a file named thishouse and prints the path to home in the file.
2. `cat doesnotexist 2>> hush.txt`
   - Explanation: Creates a file named hush.txt and prints an error saying that the file or directory doesn't exist.
3. `cat nums.txt | sort -n >> all_nums.txt`
   - Explanation: Adds the sorted version of the text in nums.txt into all_nums.txt
4. `cat << "DONE" > here.txt`
   - Explanation: Creates a file named here.txt and all text typed is added to the file until DONE is typed.
5. `ls -lt ~ | head`
   - Explanation: The first 10 lines from ls -lt are outputted.
6. `history | grep ".md"`
   - Explanation: Outputs commands in history that contain rmd or .md.

## Part 3

Verify that `roll` made it to your GitHub repository for this course and is in your `Lab03` folder.  No answers will be written here unless you would like to leave a note to the TAs

## Part 4 - Retrospective Answers

1. Where and when did it go wrong while working on your script tasks?
> Your reflection here
2. Was anything familiar working with a new language compared to one you are used to?
> Your reflection here
3. Did you write good `commit` messages that refer to what tasks were completed at each commit?  What would you improve?
> Your reflection here

## Part 5 Answers

1. PATH =
2. To set condition to `true`, I need to...
3. Command(s):
4. PATH =
   - Difference:
5. Command(s):
6. Commands & modification explanations: 
7. Script permission breakdown
   - User
      - must be:
      - has permissions to:
   - Group
      - must be:
      - has permissions to:
   - Other
      - has permissions to:

## Extra Credit

1. Note here *what* you did to the script for the extra credit.
