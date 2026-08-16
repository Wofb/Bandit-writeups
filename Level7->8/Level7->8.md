# Mission:
 Find the password in file `data.txt` next to the word `millionth`

# Steps:

 At this level, i use `grep` - a tool for **Search for PATTERNS in each FILE.**
 ### Usage: `grep [OPTION]... PATTERNS [FILE]...`
 I know that the password is next to the word `millionth`, so i will want to locate the word `millionth`.
 ```bash
 bandit7@bandit:~$ grep millionth data.txt
 ```
![Goal](Goal.png)
 The Password: `VR1ljMayciFxbnUokuQmJFw6QC9VKtub`