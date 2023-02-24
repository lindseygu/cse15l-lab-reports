## Lab Report 4: Competition Steps
### Step 1: Fork the repository
I made a fork from the original github repository given                
<img width="710" alt="Screen Shot 2023-02-23 at 4 20 22 PM" src="https://user-images.githubusercontent.com/122554943/221061199-830ba687-1184-4120-9f26-71744723e296.png">

### Step 2: log into ieng6 
Then I logged into my ieng6 account without the need to type password after the setting up process in lab. I only need to press the `return` key after typing `ssh cs15lwi23aei@ieng6.ucsd.edu`                         
<img width="809" alt="Screen Shot 2023-02-23 at 4 23 10 PM" src="https://user-images.githubusercontent.com/122554943/221061567-106627bf-6000-42fd-aca6-e620677738f5.png">

### Step 3: clone the fork of the repository using git command
I copied the ssh cloning command from the repository I forked and use `git clone <the copied link>` in the terminal              
<img width="419" alt="Screen Shot 2023-02-23 at 5 05 41 PM" src="https://user-images.githubusercontent.com/122554943/221066764-5b4e7ae9-9ec9-4357-b55a-e78732d38178.png">

<img width="569" alt="Screen Shot 2023-02-23 at 1 42 09 PM" src="https://user-images.githubusercontent.com/122554943/221061982-35d2b9c5-393e-4687-b3ba-a18aafae7a65.png">

### Step 4: run the tests and demonstrate they fail
To access the command for running the tests, I pressed `<up><up><up><up><up>`, then `<up><up><up><up><up><up>`, then `<tab>`. I first use the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command using the five up keys to search in my terminal history, then I use `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore L<tab>`using the five up keys and one tab key in the end for autofilling `TestListExamples`             
<img width="967" alt="Screen Shot 2023-02-23 at 1 42 33 PM" src="https://user-images.githubusercontent.com/122554943/221070962-6df770fd-3a8b-4014-9995-67d6220466a1.png">

### Step 5: edit the code file to fix the test
I typed `nano L<tab>` to edit the file `ListExamples.java` the `<tab>` key autocompletes the file name for me. After I entered nano, I uses `<up> <down> <left>` and `<right>` arrow keys to access different lines in the files. I made the change of the second line from `index1` to `index2` to fix the error.

<img width="422" alt="Screen Shot 2023-02-23 at 11 35 51 PM" src="https://user-images.githubusercontent.com/122554943/221119568-506f91b2-961c-4e23-a4c3-fde2fed34dd0.png">

### Step 6: run the tests and demonstrate they pass
I repeated the same steps as Step 4(but with one more `<up>`key pressed) to run the tests, and this time it passes.
<img width="980" alt="Screen Shot 2023-02-23 at 1 41 23 PM" src="https://user-images.githubusercontent.com/122554943/221072430-98c65071-a344-4697-9222-1b75c661aa73.png">

### Step 7: commit and push the change to Github account
<img width="429" alt="Screen Shot 2023-02-23 at 11 36 12 PM" src="https://user-images.githubusercontent.com/122554943/221119622-40d33aa8-6984-4582-9687-7d8e51b425f7.png">
<img width="495" alt="Screen Shot 2023-02-23 at 1 41 46 PM" src="https://user-images.githubusercontent.com/122554943/221119677-d47f146d-cba4-47b8-a1d2-3bd71683efe7.png">


