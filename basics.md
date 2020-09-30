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
string='codespeedy'  
count=0  
temp=[]  
for i in string:  
    if(i not in temp):  
        count+=1  
        temp.append(i)  
print('Total Unique Characters count:',count)    


