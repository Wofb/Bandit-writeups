# Mission
 This level is quite difficult, i have to find the password stored in a file has all of the following propeties:\
  +human-readable\
  +1033 bytes in size\
  +not executable


# Steps:
 
 ### In this level, i need to use `find` command to search the file that meet the conditions.
 First, i move in "inhere" directory
 ```bash
  cd inhere
 ```

 ### Then i list all the directories that i have, find out many folders here.
 ![Folders](Folders.png)


 ### Now i want to find exactly the file that meet all conditions:
  +human-readable\
  +1033 bytes in size\
  +not executable
 
 ```bash
 bandit5@bandit:~/inhere$ find -size 1033c -not -executable 
./maybehere07/.file2
 ```

 ### Explain the command:
  + **-size 1033c**: 1033c means 1033 bytes, 'c' for bytes, 'k' for kibibytes, 'M' for mibibytes, 'G' for gibibytes.
  + **-not -executable**: As the task requires not executable property, i have to add `-not` before `-executable`.

 ### As i see, the password is located in `./maybehere07/.file2`  path.

 ```bash
 bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
 ```

 ### The password: `pXa26xhMWaC2SvDotA4r9EgZkulOeSBW`
 


