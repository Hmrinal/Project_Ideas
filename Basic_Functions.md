# Basic Functions

## 1. Lambda()
A lambda function is a small anonymous function. It can take any number of arguments, but can only have one expression.
``` x = lambda argument:expression```
- Normal Function:   
def multiply(a,b):  
return a*b  
multiply(5,6)  
- Lambda Function:  
x=lambda a,b:a*b  
print(x(5,6))  

## 2. Map()
The map() function in Python takes in a function and a Sequence as arguments, applies the function to each item
- s=['lower','case','letters']  
upper_case= list(map(lambda a:a.upper(),s))  
print(upper_case)  
```['LOWER','CASE','LETTERS']```

## 3. Filter()
The filter() function in Python takes in a function and a Sequence as arguments
- ages =[13,90,17,59,21,60,5]  
adults=list(filter(lambda age:age>18,ages))  
print(adults)  
```[90,59,21,60]```

## 4. Reduce()
The reduce() function in Python takes in a function and a Sequence as arguments.
The reduce() function belongs to the functools module.
- from functools import reduce  
li = [5,8,10,20,50,100]  
sum = reduce((lamba x,y:x+y), li)  
print(sum)  
``` Here the results of previous two elements are added to the next element and this goes on till the end of the list like (((((5+8)+10)+20)+50)+100)```

