## Python is a multipurpose language 

- AI, ML
- Web development (along with Django) : YT, Instagram, spotify)
- Automation of repetetive tasks 

## To start with basics, we use VS code python extension

- The extension is .py 
- To run a python program with results in terminal, use CTRL+F5


## Hello World Program in python 

- Open a new folder in VS code 
- Create a new file named HelloWorld.py
- Inside the file, write : **print("Hello World")**
- Use CTRL+F5 and Hello world will be printed in the terminal (after some addresses which we need to ignore as of now)


## Modules in Python 

Python has some inbuilt modules like math. We can directly import those modules 

Other modules, we can install by using following commands in Windows powershell (open as admin) : 

pip install <module_name> // just like npm install <package name>
pip uninstall <module_name>

import math
print(math.floor(3.65))

### This will print 3 on running the file 


## Data types in python 

Similar to JS, variables can be declared as : a=1 or b="Swapnil"

print(a+" " +b) will give output as : **1 Swapnil**

### We can also get the type of variable using : print(type(3.14)). It will give result : float

### There are various functions for string : 

str1="My name is Swapnil"
print(str1.upper())

This will print : MY NAME IS SWAPNIL on the terminal 


### List data type in python 

List is a data type which is similar to array of JS but more dynamic and can store elements of different data types 

items=["Swapnil",1,true]

We can also have list within list : 

items=[1,2,3]
items2=["Swapnil",items]
print(items2[1]) // This will print : [1,2,3]


We can also change the list values : 

items2[0]="Tasvica"



### Tuple data type in python

tuple is used when we dont want out list data to change

tup1=(1,2,3)

Now we cant change the values of tuple 



### Dictionary data type in python 

Dictionary is like mapping data structure of solidity (key value pairs)

First we declare dict1 as a dictionary : 
dict1={}

And then we populate the mapping  : 
dict1["virat"] = 100
dict1["sachin"] =500

We can get the values of a key using get function : 
print(dict1.get("virat"))

We can get the list of all pairs using items function : 
print(dict1.items())

We can get the list of all keys using keys function : 
print(dict1.keys())


### Set data type 

It is the data type which doesnot all unique elements in it 

list1=[1,2,3,4,4,1]

s1=set[list1] // This is called type conversion

Then s1 = [1,2,3,4]



## Typecast in python 

a=1
b=2
c="Swapnil"

print(str(a),str(b),c)

Then, the program will print : 12Swapnil

### Here, str is an typecast operator which converts integer data type to string data type



## Handling user inputs in python 

We use the input function to take inputs from user. The default data type of input is string 

print("Enter your name")
myinput=input()
print("Your name is",myinput)

### If I want to take input in the form of integers, I will use typecast to int

print("Enter your age")
myinput=int(input())
print("You were born in",2023-myinput)




## If else conditions in python 

var1=int(input())

if(var1>2):
    print("Variable is greater")
elif(var1==2):
    print("Variable is two")
else:
    print("Variable is smaller")



## Loops in python 

for i in range(0,101):
    print(i)


i=0
while(i<101):
    print(i)
    i=i+1



### As there is no {} in python, it is designated by indent (using tab once) to show commands inside if else or the loop




## Functions in python 

def average(num1,num2):
    avr=(num1+num2)/2
    return avr

n1=int(input())
n2=int(input())

print(average(n1,n2))


### Try except block in python 

It is same as try catch block of JS 

try:
    print(index)
except Exception as e:
    print(e)


### This prints : name 'index' is not defined

This happened because index was not defined. So, instead of running into a blockhole/ error, the program returned the error message 




## File handling using python 

We use file pointers to handle create, open, edit and close a file using python 

f=open("1.txt","w") // open file in write mode 
f.write("Swapnil")
f.close()

### Code above will write in the file 

f=open("1.txt","r")
content=f.read()
f.close()
print(content)
