# Lindsey Gu's Lab Report Week1
## Installing VScode
Since I already have VScode installed on my computer, I just opened it to begin working on the Lab tasks. Here's a screenshot of what it looks like when I open the VScode:
      
<img width="666" alt="Screen Shot 2023-01-12 at 9 40 03 AM" src="https://user-images.githubusercontent.com/122554943/212140144-3b5a67a6-a90f-4342-9a11-136cf184789a.png">
       
But I will still include the process of installing VScode for future needs:   
```
1. download the correct version of VScode from the official website. I downloaded the MacOS version(see screenshot below)
2. locate the downloaded file and open it by double clicking it
3. drag the downloaded VScode app into the application folder and making it available in teh MacOS launchpad
4. double clicking VScode from the application folder to open it
5. it will look like the above screenshot and it's ready to use

```
<img width="1074" alt="Screen Shot 2023-01-24 at 6 16 59 PM" src="https://user-images.githubusercontent.com/122554943/214466648-7c7bf400-b05b-4ce8-8774-80864889f876.png">

## Remotely Connecting
I then followed the instructions to remotely connect to the server. I first signed in to my cse-specfic student account using last name and PID, I then changed the account password for this account. (later I found out that although I clicked not to change the global password of my AD account, it still changed it anyways).
            
Since I'm using a Mac, I don't need to additionally install git for Windows and using Bash. To connect with the server, I opened the terminal in VScode and typed `ssh cs15lwi23aei@ieng6.ucsd.edu`, where `cs15lwi23aei` is my student account for this class.         
           
I typed `yes` to the authenticity message and enter the new password asked, and here's what it looks like after successfully connecting.    

<img width="998" alt="Screen Shot 2023-01-12 at 8 39 10 AM" src="https://user-images.githubusercontent.com/122554943/212197197-95c0e970-14f2-4ed8-afb6-e104c4a901e0.png">

## Trying Some Commands
I tried the commands listed in the instruction to see what is returning from he server. A list of commands I tried are: 

```
cd: refers to "change directory", it's used to switch from the current working directory to the expected given path
cd ~: it changes directory to the home directory of the user, in this case, /home/linux/ieng6/cs15lwi23/cs15lwi23aei
ls -a: it list all files including the hidden ones (dotfiles)
ls -lat: it sorts files based on the recent modified time
cp /home/linux/ieng6/cs15lwi23/public/hello.txt~/: to copy the hello.txt file from current directory to the public
cat /home/linux/ieng6/cs15lwi23/public/hello.txt: to print the content in hello.txt file
ls/home/linux/ieng6/cs15lwi23/cs15lwi23aet: to list the files from the directory of another user, in this case, user cs15lwi23aet
pwd: shows the full path of the current working directory
exit: to exit the remote server; the access to cs15lwi23aei@ieng6.ucsd.edu will be closed
```
        
At first the `cp /home/linux/ieng6/cs15lwi23/public/hello.txt~/` command shows `Permission denied`. Later the TA updated and fixed the issue and then it shows the message `Hello! Welcome to CSE 15L` after I typed in `cat/home/linux/ieng6/cs15lwi23/public/hello.txt`.        
        
Here's a screenshot of all the commands I tried and the results returned from terminal:    
        
<img width="891" alt="Screen Shot 2023-01-12 at 9 19 07 AM" src="https://user-images.githubusercontent.com/122554943/212215576-ed41dc99-ac84-4db1-bea2-3a507e35b8eb.png">
