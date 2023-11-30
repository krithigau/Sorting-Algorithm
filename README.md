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
def selection_sort(nums):
    if len(nums)==6:
        for i in range(0,6):
            small=L[i]
            for j in range(i,6):
                if L[j]<=small:
                    small=L[j]
                    pos=j
            t=L[i]
            L[i]=small
            L[pos]=t
    else:
        for i in range(0,5):
            small=L[i]
            for j in range(i,5):
                if L[j]<=small:
                    small=L[j]
                    pos=j
            t=L[i]
            L[i]=small
            L[pos]=t
    return L
L= eval(input())
print(selection_sort(L))

```
ii)	#Insertion Sort
```
def insertion_sort(nums):
    # Write your code here to sort the elements in the list using Insertion sort algorithm
    if len(nums)==6:
        for k in range(1,6):
            t=list_of_nums[k]
            j=k-1
            while (j>=0 and t<=list_of_nums[j]):
                list_of_nums[j+1]=list_of_nums[j]
                j-=1
            list_of_nums[j+1]=t
        return list_of_nums
    else:
        for k in range(1,5):
            t=list_of_nums[k]
            j=k-1
            while (j>=0 and t<=list_of_nums[j]):
                list_of_nums[j+1]=list_of_nums[j]
                j-=1
            list_of_nums[j+1]=t
        return list_of_nums
    
list_of_nums = eval(input())
print(insertion_sort(list_of_nums))

```

## Output:

Selection sort:

![Alt text](<selection sort.png>)

Insertion sort:

![Alt text](<Insertion sort.png>)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
