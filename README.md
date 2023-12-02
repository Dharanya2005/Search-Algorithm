# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:DHARANYA.N
RegisterNumber:23006980
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array = eval(input())
k = eval(input())
n=len(array)
array.sort()
print(array)
result=linearSearch(array,n,k)
if result != -1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found ")

```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:DHARANYA.N
RegisterNumber: 23006980
'''
def binarysearch(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1    
array = eval(input())
array.sort()
k = eval(input())
result=binarysearch(array,k,0,len(array)-1)
print(array)
if result!=-1:
    print(f"Element found at index:  {result} ")
else:
    print(f"Element not found ")

```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: your name:DHARANYA.N
RegisterNumber:23006980
'''
def binarysearch(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1            
    return -1    
array=eval(input())
array.sort()
k=eval(input()) 
result=binarysearch(array,k,0,len(array)-1)
print(array)
if result!=-1:
    print(f"Element found at index:  {result}")
else: 
    print(f"Element not found ")

```
## Sample Input and Output

i)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/3a9289d0-4356-4863-9503-2938fe27ff13)

ii)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/fcb85c3b-5538-49b9-a5b3-2e8eb2faaeae)

iii)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/209778c7-c6c1-41e7-b963-df3f878952f0)

## OUTPUT
i)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/072e6597-fa7b-46bd-b561-f0823aa04094)

ii)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/b3e422ac-b5f8-4850-98d2-144837f10c73)

iii)
![image](https://github.com/Dharanya2005/Search-Algorithm/assets/145742468/14bb73da-59b6-430d-bac0-4784f66df0db)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
