# Sorting Exercises

### bubbleSort
* I implemented a function called bubbleSort. Given an array, bubbleSort will sort the values in the array.

- Bubble sort is an O(n^2) algorithm. You can learn about [Bubble Sort](https://www.rithmschool.com/courses/javascript-computer-science-fundamentals/basic-sorting-algorithms)
```
bubbleSort([4, 20, 12, 10, 7, 9]); // [4, 7, 9, 10, 12, 20]
bubbleSort([0, -10, 7, 4]); // [-10, 0, 4, 7]
bubbleSort([1, 2, 3]); // [1, 2, 3]
bubbleSort([]);

let nums = [
    4, 3, 5, 3, 43, 232, 4, 34, 232, 32, 4, 35, 34,
    23, 2, 453, 546, 75, 67, 4342, 32
];

bubbleSort(nums); // [2, 3, 3, 4, 4, 4, 5, 23, 32, 32, 34, 34, 35, 43, 67,
                  // 75, 232, 232, 453, 546, 4342]
```

### merge
- Given two sorted arrays, a function called merge accepts two sorted arrays and returns a new array with values from both arrays sorted.

- This function should run in O(n + m) time and O(n + m) space and should not modify the parameters passed to it.
```
let arr1 = [1,3,4,5];
let arr2 = [2,4,6,8];
merge(arr1,arr2) // [1,2,3,4,4,5,6,8]

arr1 // [1,3,4,5];
arr2 // [2,4,6,8];

let arr3 = [-2,-1,0,4,5,6];
let arr4 = [-3,-2,-1,2,3,5,7,8];

merge(arr3,arr4); // [-3,-2,-2,-1,-1,0,2,3,4,5,5,6,7,8]

let arr5 = [3,4,5]
let arr6 = [1,2]

merge(arr5,arr6) // [1,2,3,4,5]
```

### mergeSort
* I implemented the merge sort algorithm. Given an array, this algorithm will sort the values in the array. Here’s a description for how merge sort works:

- Break up the array into halves until you can compare one value with another
- Once you have smaller sorted arrays, merge those with other sorted pairs until you are back at the full length of the array
- Once the array is merged back together, return the merged (and sorted!) array
- In order to implement this function, you’ll also need to implement a merge function that takes in two sorted arrays and returns a new sorted array. I've implemented this function in the previous exercise, so I will use that function.
You can read more about [Merge Sort](https://www.rithmschool.com/courses/javascript-computer-science-fundamentals/intermediate-sorting-algorithms)
```
mergeSort([4, 20, 12, 10, 7, 9]); // [4, 7, 9, 10, 12, 20]
mergeSort([0, -10, 7, 4]); // [-10, 0, 4, 7]
mergeSort([1, 2, 3]); // [1, 2, 3]
mergeSort([]);

let nums = [
    4, 3, 5, 3, 43, 232, 4, 34, 232, 32, 4, 35, 34, 23, 2,
    453, 546, 75, 67, 4342, 32
];

mergeSort(nums); // [2, 3, 3, 4, 4, 4, 5, 23, 32, 32, 34, 34, 35,
                 //  43, 67, 75, 232, 232, 453, 546, 4342]
```

### insertionSort
* Here’s how insertion sort should work:

- Start by picking the second element in the array (we will assume the first element is the start of the “sorted” portion)
- Now compare the second element with the one before it and swap if necessary.
- Continue to the next element and if it is in the incorrect order, iterate through the sorted portion to place the element in the correct place.
- Repeat until the array is sorted.
```
insertionSort([4, 20, 12, 10, 7, 9]); // [4, 7, 9, 10, 12, 20]
insertionSort([0, -10, 7, 4]); // [-10, 0, 4, 7]
insertionSort([1, 2, 3]); // [1, 2, 3]
insertionSort([]);

let nums = [
    4, 3, 5, 3, 43, 232, 4, 34, 232, 32, 4, 35, 34, 23, 2,
    453, 546, 75, 67, 4342, 32
];

insertionSort(nums); // [2, 3, 3, 4, 4, 4, 5, 23, 32, 32, 34,
                     //  34, 35, 43, 67, 75, 232, 232, 453, 546, 4342]
```