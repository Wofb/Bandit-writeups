# Mission:
 This level require me to enter the file which having spaces in filename

# Steps:
 Using knowledge that i learn in level 1->2, i use `cat ./--spaces in this filename--` for the first try, but it wasn't work, because command can't include the spaces in the filename we enter.\
 ![Error](Error.png)
 
 Instead, using double quotes "" so the system will understand that all following inputs are the string including spaces.
 ```bash
 cat -- "--spaces in this filename--"
 ```
 
 ![Goal](Goal.png)

 ```bash
 cat ./"--spaces in this filename--"
```

![Goal2](Goal2.png)

Password: `7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME`

