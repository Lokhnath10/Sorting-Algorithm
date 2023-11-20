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
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Lokhnath.J
RegisterNumber: 23004865
'''
def selection_sort(array,size):
    for ind in range(size):
        min_index= ind
        for j in range(ind+1,size):
            if array[j] < array[min_index]:
                min_index=j
        (array[ind],array[min_index]) = (array[min_index],array[ind])
   
arr = eval(input())
size=len(arr)
selection_sort(arr,size)
print(arr)




```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: LOkhnath.J
RegisterNumber: 23004865
'''
def insertion_sort(arr):
    n=len(arr)
    if n<=1:
        return
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j -=1
        arr[j+1] = key
    
    
    
arr = eval(input())
insertion_sort(arr)
print(arr)





```

## Output:
![Screenshot 2023-11-20 024314](https://github.com/Lokhnath10/Sorting-Algorithm/assets/138969918/4fa9883e-86ef-4a73-8f62-7c1b5a2c1130)
![Screenshot 2023-11-20 024328](https://github.com/Lokhnath10/Sorting-Algorithm/assets/138969918/982b18ec-22f9-4ad7-adc7-784617296946)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
