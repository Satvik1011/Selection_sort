# Selection_sort
Selection sort is a simple and efficient sorting algorithm that works by repeatedly selecting the smallest (or largest) element from the unsorted portion of the list and moving it to the sorted portion of the list. The algorithm repeatedly selects the smallest (or largest) element from the unsorted portion of the list and swaps it with the first element of the unsorted portion. This process is repeated for the remaining unsorted portion of the list until the entire list is sorted. One variation of selection sort is called “Bidirectional selection sort” which goes through the list of elements by alternating between the smallest and largest element, this way the algorithm can be faster in some cases.

The algorithm maintains two subarrays in a given array.

The subarray which already sorted.
The remaining subarray was unsorted.
In every iteration of the selection sort, the minimum element (considering ascending order) from the unsorted subarray is picked and moved to the beginning of the sorted subarray.

After every iteration sorted subarray size increase by one and the unsorted subarray size decrease by one.
After the N (size of the array) iteration, we will get a sorted array.


Steps to solve the problem are:
1.Initialize minimum value(min_idx) to location 0.
2.Traverse the array to find the minimum element in the array.
3.While traversing if any element smaller than min_idx is found then swap both values.
4.Then, increment min_idx to point to the next element.
5.Repeat until the array is sorted.

Output
Selection sort
Time Complexity: The time complexity of Selection Sort is O(N2) as there are two nested loops:

One loop to select an element of Array one by one = O(N)
Another loop to compare that element with every other Array element = O(N)
Therefore overall complexity = O(N) * O(N) = O(N*N) = O(N2)

Auxiliary Space: O(1) as the only extra memory used is for temporary variables while swapping two values in Array. The selection sort never makes more than O(N) swaps and can be useful when the memory write is a costly operation.
