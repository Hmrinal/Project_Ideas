# Data Structures and Algorithms
## 1. Stack
Stacks are based on the LIFO principle,i.e, The element inserted at the last, is the first element to come out of the list.
- EX.  
class stack:  
```creating an empty list```  
def __init__(self):  
self.stack=[]  
``` adding an element using append```  
def push(self,x):  
self.x=x  
self.stack.append(self.x)  
print(f"{x} added to the stack.")  
``` if list is empty```  
def pop(self):  
if len(self.stack)==0:  
print("Stack Empty")  
```removing the last element using pop```  
else:  
return self.stack.pop( )  



## 2. Queue Data Structure
A queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out(FIFO)
like a one way tunnel
- EX.  
class queue:    
```creating an empty list```  
def __init__(self):  
self.queue=[]  
``` adding an element using append```  
def push(self,x):  
self.x=x  
self.queue.append(self.x)  
print(f"{x} added to the queue.")  
``` if list is empty```  
def pop(self):  
if len(self.queue)==0:  
print("Queue Empty")  
```removing the last element using pop```  
else:  
return self.queue.pop(0)  

