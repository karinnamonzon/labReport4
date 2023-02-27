# Lab Report 4

These are the following steps that will be completed:

## Setup:
1. Setup Delete any existing forks of the repository you have on your account
2. Setup Fork the repository

## Steps:
1. Log into ieng6
2. Clone your fork of the repository from your Github account
3. Run the tests, demonstrating that they fail
4. Edit the code file to fix the failing test
5. Run the tests, demonstrating that they now succeed
6. Commit and push the resulting change to your Github account

### Logging in
- Using `ssh cs15lwi23***@ieng6.ucsd.edu` (a command already saved in my terminal search history) in the terminal with `***` being replaced with my personal identification, then I log into the remote server after inputting my password when prompted then pressing `<enter>`. 
- Keys Pressed:
`<up>`
`<enter>`
[Login Image]()

### Deleting existing forks of the repository on account
Then I check if I have an existing clone of the repository using `ls` then I type `rm -rf lab7` to remove is then `<up>` and `<enter>` to call `ls` again to show that `lab7` is no longer in the remote server directory.
[setup Image]()

### Cloning the fork of the repository from Github account
Cloning the repository
I had `git clone https://github.com/karinnamonzon/lab7` saved in my terminal history so I pressed `<up>` 8 times and then `<enter>`
[Clonedlab]()

I then then I hit `<up>` and `<enter>` to call `ls` again to show that the the repository had been cloned.

I pressed `<up><up><up><up><up><up><up><up>` and `<enter>` to `cd lab7` so that I would be in the correct directory

### Checking for failed JUnit tests
Keys pressed: `<up><up><up><up><up><up><up><up><up><up><up><enter>`, `<up><up><up><up><up><up><up><up><up><up><up><enter>`

The `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was 11 up in the search history, so I used up arrow to access it. Then the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` command was 11 up in the history, so I accessed and ran it in the same way.


