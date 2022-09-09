# Quicksort
## Introduction
Quicksort is a common sorting algorithm that uses the divide and conquer technique. This algorithm sorts the numbers in-place, so there is no need for an additional array or additional memory. For quicksort, you are dividing a large array into smaller arrays, then sorting the smaller arrays. You also use a pivot element for partitioning the array. I chose to implement quicksort recursively. In summary, I learned about how quicksort works and how efficient its running time is. It is interesting to note that the running time for average and best case are the same.

## Computational running time
Best case: occurs when the partition picks the middle element as the pivot --> T(n) = 2T(n/2) + θ(n). Using case 2 of the master theorem, the running time is θ(n log n)

Worse case: occurs when the partition picks the largest or smallest element as the pivot --> T(n) = T(n-1) + θ(n). For example, we pick the first element in the array as pivot and the array is in descending order. In this case, the running time is θ(n^2)

Average case: Recurrence formula T(n) = T(n/10) + T(9n/10) + θ(n). Running time is same as best case θ(n log n).
