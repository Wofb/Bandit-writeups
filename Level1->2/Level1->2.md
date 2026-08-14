# Mission:
 Find the password located in "-" file.

# Step:
 Use `ls` to list all the file.\
 Then you will find a file "-", but when i use 
 ` cat - ` 
 nothing happen, so i google "dashed filename" as Helpful Reading Material said.\
 Google AI said "In Linux and Unix systems, a dashed filename refers to a file whose name begins with a dash or hyphen (- or --)."\
 So you have to use `cat ./-` or `cat -- -filename`.
 Before that, if your terminal is like this:
 ![Error](/
 ```bash

