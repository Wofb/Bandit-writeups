# Mission:
Find the password in file `data.txt` and is the only line of text that appears once.

# Steps:

 To find the text that appears once, i need the `uniq` command. But because `uniq` command only regconizes the repeating lines when they are next to each other, i also need to combine it with `sort` command.
 
 ## Usage:
 + `sort [OPTION]... [FILE]...`
 + `uniq [OPTION]... [INPUT [OUTPUT]]`

 ```bash
 bandit8@bandit:~$ sort data.txt | uniq -u
 ```
 ### Explain:
 + uniq -u: -u to **only print the unique line.**

 ### To combine many command, i use `|`- it's called piping.

![Goal](Goal.png)

 The password: `EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl`
