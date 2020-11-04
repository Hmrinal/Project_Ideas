# Some tricks to code differently
## 1. Swaping Variable
### Usual
a=10  
b=20  
c=a  
a=b  
b=c  
print(a,b)  
- Output: 20 10  
### Another Way
a=10  
b=20  
a,b=b,a  
print(a,b)  
- Output: 20 10
## 2. Harnessing List
### Usual
even=[]  
for i in range(10):  
  if i%2==0:  
      even.append(i)  
 print(even)  
 - Output: [0,2,4,6,8]
 ### Another Way
 even=[i for i in range(10)
        if i%2==0]  
 print(even)  
 - Output: [0,2,4,6,8]  
## 3. Lamda Function
### Usual
items=[1,2,3,4]  
def square(n):  
  return n*n  
squared=[]  
for item in items:  
  squared.append(square(item))  
print(squared)  
- Output:[1,4,9,16]
### Another Way
items=[1,2,3,4]  
squared=list(map(lambda x:x**2,items))
print(squared)
- Output:[1,4,9,16]
## 4. The python debugger
- for big projects
def add(a,b):  
  print(a+b)
add(1,2) - output: 3
import pdb
pdb.set_trace()
```pauses the execution and helps you to debug and identify the problem```
add(1,'two') - output: gives error
## 5. List and Dict Compression
### Usual
fruits=[  
         {'name':'apple',  
         'color':'red'},  
         {'name':'banana',  
         'color':'yellow'},]  
fruit_name=[]  
for fruit in fruits:  
  fruit_name.append(  
    fruit['name'])  
print(fruit_name)  
### Another Way
fruits=[  
         {'name':'apple',  
         'color':'red'},  
         {'name':'banana',  
         'color':'yellow'},]  
fruit_name=[fruit['name'] for fruit in fruits]  
print(fruit_name)  
- output:['apple','banana']  
## 6. Print Emojies
!pip install emoji  
from emoji import emojize  
print(emojize(":thumbs_up:"))  
- Output: :thumbsup:
## 7. Instant Stack Overflow
!pip install howdoi  
!howdoi for loop in PYTHON  
``` output:```  
```mylist=[1,2,3]```  
```for item in mylist:```  
  ```print item```  
```mydict={1:'one',2:'two',3:'three'}```  
```for key in mydict:```  
  ```print key, mydict[key] ```    
note: it scrapes code from top answers from StackOverflow. It might not always give the most helpful information 
  
