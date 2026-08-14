#Mission: 
 ###Connect to the bandit server using SSH and find the password in readme file.

#Step: 
 Using ssh to connect to the server: 
  ```bash
  ssh bandit0@bandit.labs.overthewire.org -p 2220
  ```
 Enter the password: `bandit0`
 Using `ls` command to list the files in the directory, you will find a file named `readme`. Use the `cat` command to read the contents of the file and find the password for the next level.   
 ```bash
    cat readme
 ```
 
 

