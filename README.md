# notes-bash

## unix thing
```python
#!/bin/bash
```

## Select Statement
#### compare integers
```python
num -eq 9 #equal to
num -ne 9 #not equal to
num -lt 9 #less than
num -le 9 #less than and equal to 
num -gt 9 #greater than
num -ge 9 #greater than and equal to 
```

#### compare strings
```python
str == "wassup" #equal to 
str != "wassup" #not equal to 
str < "wassup"  #less than, although I dont get it
str > "wassup"  #greater than
```

####checking files
```python
-e file #if a file exists or not, probably when you want to read data from a file
-f file #whether it is a file in first place
-d file #directory
-s file #any data inside
-r file #readable
-w file #writable
-x file #excecutable
#and so on...
```

##case
```python
var=$1
case $var in
  "dog")
    echo "Woof!"
    echo "(Matched First)";;
 "cat" | "kitty")
    echo "Meow!"
    echo "(Matched Second!)";;
 *)
    echo "No idea!";;
esac
```

##arithmatic
```python
a = a*25
```

####for decimal stuff
```python
echo "scale=2; 1/2" | bc #dont forget the bc and scale
echo "scale=21; 1/2" | bc 
```

##exit code
```python
exit 1 #indicate error or succesful build for the next command to know
```

##array
```python
name[66] = "Joe"
name[32] = "John"
name[12] = "Jimbo"

echo ${name[66]} #curly bracket and the dollar

names2= ([12]="Jimbo" [66]="Joe" [32]="John") #specific index
```

