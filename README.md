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

##iteration

```python
#!/bin/bash
for (( i=1 ; i<=5 ; i++ )) #take care of the exact spacing
do
  echo $i
done

for i in 1 2 3 4 5 6 7 8 9 10 11 12 100 #nutcase
do
  echo $i
done

for i in seq 0 5 20 #did not actually work for me
do
  echo $i
done

for i in $(ls) #the list dont have to be always number
do
  echo $i
done

```

##functions
```python
showtime() ##no need for the "def" or "function" before it. The "()" does the job
{
        echo `date +"%1:%M%P"`
        return #need to mention the return
}
showtime #no need of the brackets to call the func
```

##internal variables
```python
$BASH_VERSION #got to be captial letters
$BASH_UID #id can be pretty useless
$FUNCNAME #its func not function
$HOME #home directory
$HOSTTYPE #integrated chips stuff
$OSTYPE #linux or ms
$PWD #pretty handy
$SECONDS #has got to be in micro sec
$LINENO #for debuggin i guess

```





