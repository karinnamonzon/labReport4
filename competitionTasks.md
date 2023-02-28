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

---

### Logging in
- Using `ssh cs15lwi23***@ieng6.ucsd.edu` (a command already saved in my terminal search history) in the terminal with `***` being replaced with my personal identification, then I log into the remote server after inputting my password when prompted then pressing `<enter>`. 
- Keys Pressed:
`<up>`
`<enter>`
![Login Image](https://github.com/karinnamonzon/labReport4/blob/main/login.png?raw=true)

---

### Deleting existing forks of the repository on account
Then I check if I have an existing clone of the repository using `<up><up><up><up><enter>` to get to the command`ls` then I typed `rm -rf lab7` to remove is then `<up>` and `<enter>` to call `ls` again to show that `lab7` is no longer in the remote server directory.
![setup Image](https://github.com/karinnamonzon/labReport4/blob/main/setup.png?raw=true)

---

### Cloning the fork of the repository from Github account
Cloning the repository
I had `git clone https://github.com/karinnamonzon/lab7` saved in my terminal history so I pressed `<up>` 8 times and then `<enter>`
![Clonedlab](https://github.com/karinnamonzon/labReport4/blob/main/clonedLab.png?raw=true)

I then then I hit `<up><enter>` to call `ls` again to show that the the repository had been cloned.

I pressed `<up><up><up><up><up><up><up><up><enter>` to `cd lab7` so that I would be in the correct directory `lab7`  where the JUnit tests would be run.

---

### Checking for failed JUnit tests
Keys pressed: `<up><up><up><up><up><up><up><up><up><up><up><enter>`, `<up><up><up><up><up><up><up><up><up><up><up><enter>`

The `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was 11 up in the search history, so I used up arrow to access it. Then the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command was 11 up in the history, so I accessed and ran it in the same way.

![JUnittests1fail](https://github.com/karinnamonzon/labReport4/blob/main/JUnittesting1fail.png?raw=true)

---

### Debugging code to fix failing test

The bug was in the file `ListExamples.java` 
Using `<up><up><up><up><up><up><up><up><up><up><up><up><up><up><enter>` to get to the command `nano ListExamples.java`. Nano is called and this allows me to see the file `ListExamples.java`. 

![Nanocall](https://github.com/karinnamonzon/labReport4/blob/main/nanoCall.png?raw=true)

Following is key presses to make changes in `ListExamples.java`
- `<^O><enter>`
- `<^W><index1><enter>`
- `<down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down>` (17 times)
- `<right><right><right><right><backspace> 2`
- `<^X>` y `<enter>`

Changes made in `merge` after saving in nano:
![ChangesinNano](https://github.com/karinnamonzon/labReport4/blob/main/changesMadeNano.png?raw=true)

It was a change of one character from `index1` to `index2`.

---
 
### Run JUnit tests to show that they succeed
Keys pressed: `<up><up><up><enter>`, `<up><up><up><enter>`
 
Since the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was saved in my search terminal I pressed `<up>` three times to get to the command then the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command was 3 up in the history, so I accessed and ran it in the same way.

Here are the results of running the JUnit tests. It now says that the two tests passed. 
![2correct](https://github.com/karinnamonzon/labReport4/blob/main/2correct.png?raw=true)

---
  
### Commit and push changes to Github account
Keys pressed: 
- `<up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><enter>` (16 up, 1 enter)
- `<up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><enter>` (16 up, 1 enter)
- `<up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><enter>` (16 up, 1 enter)
- `<up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><up><enter>` (16 up, 1 enter)
- `cd<space><~><enter>`
- `rm<space><->rf<space>lab7 <enter>`
- `<exit><enter>`

I had the command `git add ListExamplesTests.java ListExamples.java`in my history so I pressed <up> 16 times and then enter to run it and add these files to my GitHub. Then the command git `commit -m "Successful commit"` was run by a command saved in my history and accessed that the same way and pressed `<enter>`, this shows that I had commit changes to GitHub. The next command was `git commit` which was saved in my history that was accessed in the same way, this allowed for changes to be fully committed. The next command was `git push` which was a stored command in the terminal history and this allowed for all changes that had been committed to be pushed to the repository. I then used `cd ~` by typing into hte terminal in order to go to the home director in order to remove the `lab7` directory by typing 'rm -rf lab7` for the next log-in. Then I typed `exit` to exit the remote server completely.

Calling command `git commit` and its results
  ![gitCommit](https://github.com/karinnamonzon/labReport4/blob/main/gitCommit.png?raw=true)
  
Calling command `git add` and its results. Removing `lab7` and then exiting from the remote server.
  ![gitPush](https://github.com/karinnamonzon/labReport4/blob/main/gitpush.png?raw=true)
