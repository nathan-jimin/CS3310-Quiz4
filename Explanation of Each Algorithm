# CS3310-Quiz4
Peaks and Valleys + Build Order Project for CS 3310:  Design and Analysis of Algorithms

Peaks and Valley Explanation
Looking at the problem, I have noticed that since peaks and valleys work as min -> max -> min -> ... , I can sort the array first and place the maximum value (index = n) in another array with the same length at index = 0, n - 1 index at index 3, and so on until I reach the end of the array. Then I place the minimum value (index = 0) in the second array's index 1, min value index + 2 at second array's index 3, and so on until I reach the end. This creates the pattern of peak (max index), valley (min index), peak (max index - 1), valley (min index + 1) and so on until the second array is filled.

The basic operation of this algorithm would be placing an element from the first array into another array.
Input size is the amount of elements in the first array.
The order of the peaks and valley sort is O(n) since the first array must be run through only once, placing a value at a certain index in another array. If we are to include the sorting algorithm (in which we can assume the fastest algorithm (eg. mergesort or quicksort)) then the order of the sort would be O(n) + O(nlogn), which reduces to O(nlogn).

Build Order Explanation
The projects and dependencies can be seen as a sort of directed graph when drawn out. I noticed that following the build order from the example would lead to a depth-first search of this said graph. Starting from project A (or 0 in the code), I traverse the graph and place temporary marks on each visited project if connected by a "dependency". If the project has no other dependencies, traverse back up the graph, placing a permanent mark while placing it in a list and removing the temporary mark from each project, until the original project is reached. Do this until every project has a permanent mark or a traversal reaches a project that already has a temporary mark.

Basic operation of this algorithm is placing a permanent mark on a project when traversing the graph
Input size is the amount of projects.
The order of this algorithm would be O(n) since this is a modified version of depth-first search, which also has an order of O(n). The projects do not need to be sorted whatsoever, meaning there is no other order to consider for this algorithm.
