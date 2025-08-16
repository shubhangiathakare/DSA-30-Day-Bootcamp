# 📘 Day 03: Topic Sorting Algorithms

### ✅ Summary:
- 1. Bubble Sort

Idea:
Repeatedly compare adjacent elements.
If they are in the wrong order, swap them.
Largest element “bubbles” to the end after each pass.

Steps:
Start from the first element.
Compare arr[i] and arr[i+1].
Swap if arr[i] > arr[i+1].
Repeat until no swaps are needed.

Example:
Array = [5, 3, 4, 1]
Pass 1 → [3, 4, 1, 5
Pass 2 → [3, 1, 4, 5]
Pass 3 → [1, 3, 4, 5] ✅ Sorted

Complexity:
Best Case: O(n) (already sorted, 1 pass)
Worst Case: O(n²) (completely reversed)
Space: O(1) (in-place)

Use Case:
Good for small arrays or when array is nearly sorted.
Easy to implement but inefficient for large data.

2. Insertion Sort

Idea:
Builds the sorted array one element at a time.
Similar to sorting playing cards in your hand.

Steps:
Start from index 1.
Compare the element with the left part (which is already sorted).
Insert it into the correct position.

Example:
Array = [5, 3, 4, 1]
Step 1 → [3, 5, 4, 1]
Step 2 → [3, 4, 5, 1
Step 3 → [1, 3, 4, 5] ✅ Sorted

Complexity:
Best Case: O(n) (already sorted)
Worst Case: O(n²)
Space: O(1) (in-place)

Use Case:
Efficient for small arrays (better than Bubble/Selection).
Useful for online algorithms (insert new elements dynamically).

3. Selection Sort

Idea:
Select the smallest (or largest) element in each pass.
Place it at the beginning of the unsorted portion.

Steps:
Find the minimum element.
Swap it with the first element.
Repeat for the remaining unsorted array.

Example:
Array = [5, 3, 4, 1]
Pass 1 → [1, 3, 4, 5]
Pass 2 → [1, 3, 4, 5]
Pass 3 → [1, 3, 4, 5] ✅ Sorted

Complexity:

Best, Worst, Average: O(n²)
Space: O(1)
Use Case:
Works well for small datasets.
Not adaptive (doesn’t improve with partially sorted data).

4. Merge Sort

Idea:
Uses Divide & Conquer strategy.
Recursively splits the array into halves, sorts them, then merges.

Steps
Divide array into 2 halves.
Sort each half recursively.
Merge sorted halves.

Example:
Array = [5, 3, 4, 1]
Split → [5, 3] & [4, 1]
Sort → [3, 5] & [1, 4]
Merge → [1, 3, 4, 5] ✅ Sorted

Complexity:
Best, Worst, Average: O(n log n)
Space: O(n) (extra space for merging)

Use Case:

Efficient for large datasets
Preferred when stability is required (preserves order of equal elements).

Comparison Table:

Algorithm	  |  Best Case	|  Worst Case	 |   Space	 Stable?
Bubble Sort   |	O(n)	    |   O(n²)	     |  O(1)	|✅ Yes
Insertion Sort|	O(n)	    |  O(n²)	     |  O(1)	|✅ Yes
Selection Sort| O(n²)	    |  O(n²)	     |  O(1)	|❌ No
Merge Sort	  | O(n log n)  | O(n log n)      |	O(n)	| ✅ Yes


### 🔗 Problems:
1. 
