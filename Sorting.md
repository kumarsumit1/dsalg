
# Sorting Terminology

- In-place sorting : An in-place sorting algorithm uses constant extra space for producing the output (modifies the given array only). It sorts the list only by modifying the order of the elements within the list.
    Insertion Sort and Selection Sorts are In-place sorting algorithms
    Merge Sort and Count Sort are NOT In-place sorting algorithms

- Internal and External Sortings : When all data that needs to be sorted cannot be placed in-memory at a time, the sorting is called external sorting. External Sorting is used for massive amount of data. When all data is placed in-memory, then sorting is called internal sorting.

    ***Merge Sort is usually used for External Sorting.***    
 
In the sorting phase, chunks of data small enough to fit in main memory are read, sorted, and written out to a temporary file. In the merge phase, the sorted sub-files are combined into a single larger file. 

- Stable sorting : A sorting algorithm is said to be stable if two objects with equal keys appear in the same order in sorted output as they appear in the input array to be sorted.

    Stability is mainly important when we have key value pairs with duplicate keys possible (like people names as keys and their details as values). And we wish to sort these objects by keys. 

Note : ***When equal elements are indistinguishable, such as with integers, or more generally, any data where the entire element is the key, stability is not an issue. Stability is also not an issue if all keys are different.***

Some Sorting Algorithms are stable by nature, such as Bubble Sort, Insertion Sort, Merge Sort, Count Sort etc.

Quick Sort, Heap Sort etc. are by default not stable in nature.

In general any algorithm can be made stable by applying an additional step of sorting the values but that may add to overhead.

# Time Complexity
|    Algorithm   |             | Time Complexity |             |
|:--------------:|:-----------:|:---------------:|:-----------:|
|                |     Best    |     Average     |    Worst    |
| Selection Sort |    Ω(n^2)   |      θ(n^2)     |    O(n^2)   |
|   Bubble Sort  |     Ω(n)    |      θ(n^2)     |    O(n^2)   |
| Insertion Sort |     Ω(n)    |      θ(n^2)     |    O(n^2)   |
|    Heap Sort   | Ω(n log(n)) |   θ(n log(n))   | O(n log(n)) |
|   Quick Sort   | Ω(n log(n)) |   θ(n log(n))   |    O(n^2)   |
|   Merge Sort   | Ω(n log(n)) |   θ(n log(n))   | O(n log(n)) |
|   Bucket Sort  |    Ω(n+k)   |      θ(n+k)     |    O(n^2)   |
|   Radix Sort   |    Ω(nk)    |      θ(nk)      |    O(nk)    |