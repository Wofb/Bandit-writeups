# Mission
 This level require me to find the password located in a hidden file in the "inhere" directory

# Steps:

 First, i use `cd inhere` to change directory.\
 Because the file is hiddened, so if i use `ls`, nothing appear.

 ![Attempt](Attempt.png)

 So i have to use `ls -a` aka list all to list all the files, including hidden file.

 ```bash
  ls -a
 ```
 ![Hidden file](HiddenFile.png)
 
 Now i know that the hidden file is `...Hiding-From-You`.
 ```bash
 cat ...Hiding-From-You
 ```
![Goal](Goal.png)

 The password: `xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq
`

 