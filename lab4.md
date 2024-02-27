## Lab Report 4

### Steps 4 through 9 of lab7 reproduced
Summarize commands and explain what effect keypresses had

**Step 4**
![Step4](lab4screenshotstep4.jpeg)
Here I logged into ieng6 using `ssh soxlaj@ieng-202.ucsd.edu` command (not apparent in the screenshot but was later used because of issues with default `ieng6-203`) and this command essentially allows me to log in remotely to a server.  

**Step 5**
![Step5](lab4screenshotstep5.jpeg)
In this step, I cloned the `ssh` link of the fork of the repository of lab7 using `git clone <link>`. while in the ieng6 server and so this creates a clone on the remote server of the fork of the lab7 repository. Here, if you use `ls` we will see `lab7` as a file in the working directory, and for the next step we `cd` into `lab7` to work on this clone.

**Step 6**
![Step6](lab4screenshotstep6-2.jpeg)
In this step, I had already ran these tests before and so I used the arrow keys (up) to access the same commands. The keys pressed were:
`<up><up><up><up><enter>` and `<up><up><up><up><enter>`
We reaccessed `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamples.java` using the arrow keys in the sequence above to access them from the history. This access compiles and runs the JUnit tests and displays the tests failing from an error in the code. 

**Step 7**
![Step7](lab4screenshotstep7vim.jpeg)
In this step, as evident in the screenshot above, we enter `vim` mode using the command `vim ListExamples.java` to enter into vim and fix the error in the code found within the java file `ListExamples`. The `vim` command allows us to access and edit files from the terminal and in this instance allows us to access and edit the file `ListExamples.java` that is cloned in the remote server and to fix the error. 
Entering `vim` displays the output above, and in this we are in `normal mode` in which we use the arrow keys to navigate through the lines of code however we cannot make changes. To make a change, we need to use enter `insert mode` where we can edit the characters in the file using keys and the set of keys we use to fix the error in the code are the following:
`<down>(43 times)<e><right><backspace><2>`
And this changes the character that caused the tests to fail, and to exit `insert mode` we use the keys:
`<esc>`
Leaving `insert mode` and entering `normal mode` we can now save and quit vim using the keys:
`<shift>+<;><w><q>`
In which the key `w` saves the changes made in `vim` and `q` exits out of `normal mode` and `vim` thus saving the change to the `ListExamples.java` file.

**Step 8**

![Step8](lab4screenshotstep8.jpeg)

**Step 9**
![Step9](lab4screenshotstep9-1.jpeg)

![Step9](lab4screenshotstep9-2.jpeg)

![Step9](lab4screenshotstep9-3.jpeg)
