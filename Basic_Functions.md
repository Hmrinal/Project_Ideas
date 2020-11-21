# Basic Functions

## 1. Lambda
A lambda function is a small anonymous function. It can take any number of arguments, but can only have one expression.
``` x = lambda argument:expression```
- Normal Function:   
def multiply(a,b):  
return a*b  
multiply(5,6)  
- Lambda Function:  
x=lambda a,b:a*b  
print(x(5,6))  

## 2. Map
The map() function in Python takes in a function and a Sequence as arguments, applies the function to each item
- s=['lower','case','letters']  
upper_case= list(map(lambda a:a.upper(),s))  
print(upper_case)  
```['LOWER','CASE','LETTERS']
