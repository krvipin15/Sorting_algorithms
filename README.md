# Sorting algorithms
A Sorting Algorithm is used to rearrange a given array or list elements according to a comparison operator on the elements. The comparison operator is used to decide the new order of elements in the respective data structure.

## Bubble sort
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in the wrong order. This algorithm is not suitable for large data sets as its average and worst-case time complexity is quite high.\
Time Complexity: O(N^2)\
Auxiliary Space: O(1)

```
def bubble(arr):
    for iter_num in range(len(arr)):
        for i in range(len(arr) - 1 - iter_num):
            if arr[i] > arr[i + 1]:
                arr[i], arr[i + 1] = arr[i + 1], arr[i]
arr = [87, 65, 89, 3, 54, 12, 67]
bubble(arr)
```

## Selection sort
The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning. The algorithm maintains two subarrays, first, subarray which is already sorted and remaining subarray which is unsorted.\
Time Complexity: O(N^2)\
Auxiliary Space: O(1)

```
def selection(arr):
    for iter_num in range(len(arr)):
        for i in range(iter_num + 1, len(arr
            if arr[i] < arr[iter_num]:
                arr[i], arr[iter_num] = arr[iter_num], arr[i]

arr = [87, 65, 89, 3, 54, 12, 67]
selection(arr)
```

## Insertion sort
Insertion sort is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.\
Time Complexity: O(N^2)\
Auxiliary Space: O(1)

```
def insertion(arr):
    for iter_num in range(1, len(arr)):
        curr = arr[iter_num]
        pointer = iter_num - 1
        while pointer >= 0 and curr < arr[pointer]:
            arr[pointer + 1] = arr[pointer]
            pointer -= 1
        arr[pointer + 1] = curr

arr = [87, 65,89,3, 54, 12,67]
insertion(arr)
```

## Merge Sort
The Merge Sort algorithm works on divide and conquer strategy. So, in this algorithm, the array is initially divided into two equal halves and then they are combined in a sorted manner. We can think of it as a recursive algorithm that continuously splits the array in half until it cannot be further divided. This means that if the array becomes empty or has only one element left, the dividing will stop, i.e. it is the base case to stop the recursion. If the array has multiple elements, we split the array into halves and recursively invoke the merge sort on each of the halves. Finally, when both the halves are sorted, the merge operation is applied. Merge operation is the process of taking two smaller sorted arrays and combining them to eventually make a larger one.\
Time Complexity: O(n log(n))\
Auxiliary Space: O(n)

```
def merge(arr):

```
