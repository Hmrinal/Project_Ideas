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
