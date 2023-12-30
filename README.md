# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```

''' 
Program for linear search method to match the item in a list
Developed by: TH KARTHIK KRISHNA
RegisterNumber: 23014165
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i] == k):
            return i
    return -1
    
array = eval(input())
k = eval(input()) 
n= len(array)
array.sort()
result = linearSearch(array,n,k)
if(result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)





```
ii)	#Insertion Sort
```


''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by: TH KARTHIK KRISHNA
RegisterNumber: 23014165
'''
def binarySearchIter(array, k, low, high):
    while low <= high:
        mid =low + (high - low)//2
        if array[mid] == k:
            return mid
            
        elif array[mid] < k:
            low = mid + 1
        else:
            high = mid - 1
    return -1
array = eval(input())
array.sort()
k = eval(input())
result = binarySearchIter(array, k, 0, len(array)-1)
if(result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
    



```

## Output:
![Screenshot 2023-12-30 230010](https://github.com/karthikkrishna16/Sorting-Algorithm/assets/148514663/eeb38ae7-df8b-49d2-b08f-849a8d0a7003)

![Screenshot 2023-12-30 230043](https://github.com/karthikkrishna16/Sorting-Algorithm/assets/148514663/c322f3bd-951a-41af-9c99-4a12bd9d7a39)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
