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
