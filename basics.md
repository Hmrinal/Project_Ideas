# Important Basics 
## 1. Reverse Matrix  
eg.[[1,2],[3,4],[5,6]]--> [[6,5],[4,3],[2,1]]  
Sol. >>> grid=[[1,2,[3,4],[5,6]]  
     >>> [lst[::-1] for lst in grid[::-1]]
## 2. Checking Subset
A = {1, 2, 3}  
B = {1, 2, 3, 4, 5}  
Sol. it uses 'issubset'
- Returns True
- print(A.issubset(B))
## 3. Counting unique charaters
- unique char total count
string='codespeedy'  
count=0  
temp=[]  
for i in string:  
    if(i not in temp):  
        count+=1  
        temp.append(i)  
print('Total Unique Characters count:',count)  
output: Total Unique Characters count:7  
- Unique occurance with letter and count
def char_frequency(str1):  
    dict = {}  
    for n in str1:  
        keys = dict.keys()  
        if n in keys:  
            dict[n] += 1  
        else:  
            dict[n] = 1  
    return dict  
print(char_frequency('google.com'))  
output: {'g': 2, 'o': 3, 'l': 1, 'e': 1, '.': 1, 'c': 1, 'm': 1}  


