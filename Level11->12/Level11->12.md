# Mission:
 Find the password in data.txt, where all the characters in this file have been rotated by 13 positions.

# Steps:

 I will peek in this file too see what is inside.
 ```bash
  bandit11@bandit:~$ cat data.txt
  Gur cnffjbeq vf TEBbmJCB8DlA0zTewHxVQ0JPLxMvDkeA
 ```

 As discription, the lowercase(a-z) and uppercase(A-Z) have been move 13 positions, and because the alphabet have 26 letters, so if i shift all the letters by 13 positions again, it will returns to its orginal position.

 ### To move the characters, i use `tr` command 

 ## Usage:
 + `tr [OPTION]... SET1 [SET2]`

 ```bash
  bandit11@bandit:~$ cat data.txt | tr 'N-ZA-Mn-za-m' 'A-Za-z'
 ```

 ## Explain the code:
 + `|`: use piping to combine `cat` command and `tr` command
 + `N-ZA-Mn-za-m` -> `A-Za-z`: move the characters in ranges "N->Z + A->M" in uppercase and lowercase to "A->M + N->Z"(in short "A->Z").

 ![Goal](Goal.png)

 The password: `GROozWPO8QyN0mGrjUkID0WCYkZiQxrN`

