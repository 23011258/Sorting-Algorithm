# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
# step1:
using def selection_sort(nums) ,we start the program
# step2:
using for loop and if condition we will continue the program
# step3:
giving input for list of nums
# step4:
sorting out the list of nums
# step5:
printing the list of nums

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
Developed by: Chandana Yendluri
RegisterNumber: 23011258
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)

```
## input and output
![image](https://github.com/23011258/Sorting-Algorithm/assets/139842204/a7ce54a8-aa7a-4376-a14a-4088f421d05e)

ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Chandana Yendluri
RegisterNumber: 23011258
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
# use the selection sort function
# print the sorted list
```
## input and output:
![image](https://github.com/23011258/Sorting-Algorithm/assets/139842204/048bcc12-a4fc-4e11-9816-d42a0b47b4dd)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
