# Lindsey Gu's Lab Report Week1
## Installing VScode
Since I already have VScode installed on my computer, I just opened it to begin working on the Lab tasks:

<img width="666" alt="Screen Shot 2023-01-12 at 9 40 03 AM" src="https://user-images.githubusercontent.com/122554943/212140144-3b5a67a6-a90f-4342-9a11-136cf184789a.png">

## Remotely Connecting
I then followed the instructions to remotely connect to the server. I first signed in to my cse-specfic student account using last name and PID, I then changed the account password for this account. (later I found out that although I clicked not to change the global password of my AD account, it still changed it anyways).
            
Since I'm using a Mac, I don't need to additionally install git for Windows and using Bash. To connect with the server, I opened the terminal in VScode and typed `ssh cs15lwi23aei@ieng6.ucsd.edu`, where `cs15lwi23aei` is my student account for this class.         
           
I typed `yes` to the authenticity message and enter the new password asked, and here's what it looks like after successfully connecting.    

<img width="998" alt="Screen Shot 2023-01-12 at 8 39 10 AM" src="https://user-images.githubusercontent.com/122554943/212197197-95c0e970-14f2-4ed8-afb6-e104c4a901e0.png">

## Trying Some Commands
I tried the commands listed in the instruction to see what is returning from he server. A list of commands I tried are: 

```
cd
cd ~
ls -a
ls -lat
cp /home/linux/ieng6/cs15lwi23/public/hello.txt~/
cat /home/linux/ieng6/cs15lwi23/public/hello.txt
ls/home/linux/ieng6/cs15lwi23/cs15lwi23aet
pwd
exit
```
        
At first the `cp /home/linux/ieng6/cs15lwi23/public/hello.txt~/` command shows `Permission denied`. Later the TA updated and fixed the issue and then it shows the message `Hello! Welcome to CSE 15L` after I typed in `cat/home/linux/ieng6/cs15lwi23/public/hello.txt`.        
        
Here's a screenshot of all the commands I tried and the results returned from terminal:    
<img width="891" alt="Screen Shot 2023-01-12 at 9 19 07 AM" src="https://user-images.githubusercontent.com/122554943/212215576-ed41dc99-ac84-4db1-bea2-3a507e35b8eb.png">
