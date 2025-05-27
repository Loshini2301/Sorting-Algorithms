# Selection sort and Insertion sort
## NAME:LOSHINI G
## REGISTER NO:212223220051
## DEPARTMENT:IT
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
# Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Loshini G
RegisterNumber: 23012268
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)    
list_of_nums = eval(input())
selection_sort(list_of_nums)




```
# Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Loshini G
RegisterNumber: 23012268
'''
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1

        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1
        
        arr[j + 1] = key
    
    return arr
    
l=eval(input())
print(insertion_sort(l))






```

## Output:
![image](https://github.com/user-attachments/assets/f4e71193-b76c-4e74-bd28-a388861c3384)
![image](https://github.com/user-attachments/assets/2233e5c5-9247-48e9-a326-c51ed48c9833)
![image](https://github.com/user-attachments/assets/9eca1ec6-4377-4a95-9dd7-81d93021cf69)
![image](https://github.com/user-attachments/assets/d5aef9fe-f379-4824-85fb-fb6c18b2a945)




## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
