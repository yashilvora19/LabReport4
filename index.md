# Lab Report 4

## Commands Run in the Lab Competition

This lab report will take a closer look at all of the commands run in the lab competition and how I used shortcuts to complete alal the tasks quickly as I could.
For the competition, I had to complete the following tasks: 

1. **Setup** Delete any existing forks of the repository you have on your account
2. **Setup** Fork the repository
3. **The real deal** Start the timer!
4. Log into ieng6
5. Clone your fork of the repository from your Github account
6. Run the tests, demonstrating that they fail
7. Edit the code file to fix the failing test
8. Run the tests, demonstrating that they now succeed
9. Commit and push the resulting change to your Github account (you can pick any commit message!)

For the purposes of this report, we will start fromm step 4 and assume that the setup is already completed. 

### 4. Log into ieng6

_Keys pressed:_ 
`<up><enter>`

Since I had typed this in previously and it was the last command before logging into ieng6, I just had to press the up arrow to access it and pressed the enter 
key to run the command which came up (`ssh cs15lwi23aqv@ieng6.ucsd.edu`). Since the ssh key was setup, I wasn't prompted for a password and was automatically 
logged in.

### 5. Clone your fork of the repository from your Github account

_Keys pressed:_ 
`<ctrl><r>git c<enter>`

Pressing the control and r keys together allow me to search for commands in my history. Typing `git c` was enough for the entire command `git clone git@github.com:yashilvora19/lab7.git` to show up. After this, I just had to press the enter key for it to execute the commmand and clone the repository into the ieng6 server. 

### 6. Run the tests, demonstrating that they fail

_Keys pressed (for compiling files):_ 

`cd lab7`
`<ctrl><r>javac<enter>`

I first changed my directory to lab7 using `cd lab7` so that I could compile and run the files successfully. To compile all files in the directory, I ran `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`. I used the ctrl+r command once again to search for the `javac` command. On finding it, I pressed enter and ran the command. Note: Ending with `*.java` makes sure that all files in the current directory are compiled together.

_Keys pressed (for running tests):_ 

`<ctrl><r>java <enter>`

I used ctrl+r to find the java command in my history. On finding `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples`, I clicked on the enter button to run the tester file. The output of this showed that one of the tests failed and needed to be fixed.

### 7. Edit the code file to fix the failing test

_Keys pressed:_ 

`nano L<tab>.java<enter>`
`<ctrl><w>index1 +=<enter><down><down><down><down><right><right><right><right><right><right><backspace>2`
`<ctrl><x>Y<enter>`

The first command opened up the file in the terminal so that I could fix the bug. Pressing the tab button autocompleted the file name. Since there were 2 `ListExamples` files (one with a `.java` extension and one with a `.class` extension, I had to type in `java` in order to make sure I open the correct file). 

Once I opened up the file in the terminal, I knew which part I needed to edit and so used the search command in nano by pressing the ctrl and w keys together. I searched for `index1 +=` and clicked on enter. This went to the the first instance of this string in the file. However, that wasn't the one I needed to edit, and so I had to navigate down by 4 lines (which I did by clicking the down button 4 times) and change the "index1" to "index2" (which I did by clicking on the right button 6 times, clicking on the backspace button once, and typing 2). 

To save these changes, pressed ctrl+x to exit the file. I was prompted with a message asking whether I wanted to save the changes. I typed "Y" and pressed enter to save this. This is how I editted the code to fix the failing test.

### 8. Run the tests, demonstrating that they now succeed

_Keys pressed (for compiling files):_ 
`<ctrl><r>javac<enter>`

To compile all files in the directory once again, I ran `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`. I used the ctrl+r command once again to search for the `javac` command. On finding it, I pressed enter and ran the command. Note: Ending with `*.java` makes sure that all files in the current directory are compiled together.

_Keys pressed (for running tests):_ 
`<ctrl><r>java <enter>`

I used ctrl+r to find the java command in my history. On finding `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples`, I clicked on the enter button to run the tester file. This time, the output showed that all the tests passed and that there were no failures.

### 9. Commit and push the resulting change to your Github account (you can pick any commit message!)

_Keys pressed:_ 

`<ctrl><r>git a<enter>`
`<ctrl><r>git c<enter>`
`<ctrl><r>git p<enter>`

This step was done by runnning 3 commands. The first command found `git add ListExamples.java` in my history, and running it added the change in the working directory to the staging area. 

The second command found `git commit -m "[FIXED]"` in my history, and saved the changes made to my local repository with the message "[FIXED]".
 
 Lastly, running the third command found `git push` in my history, and running it uploaded local repository content to a remote repository.
 
 All 3 of these commands had a successful output in the terminal and the changed were successfully committed and pushed to Github.
 
## Conclusion

This lab helped me find a lot of ways to make my workflow more efficient in the terminal. I became more accustomed to running commands in the terminal and was able to complete all the tasks very quickly.
 
