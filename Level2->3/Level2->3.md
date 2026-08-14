# Mission:
 This level require me to enter the file which having spaces in filename

# Steps:
 Using knowledge that i learn in level 1->2, i use `cat ./--spaces in this filename--` for the first try, but it wasn't work, because `./` command don't include the spaces in the filename we enter.\
 ![Error](Error.png)
 
 Instead, using `--` so the system will understand that all following inputs are the names, combine with the doule quote "" to treat the spaces as literal character.   
 ```bash
 cat -- "--spaces in this filename--"
 ```

 ![Goal](Goal.png)

Password: `7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME`