# 📘 Day 02:  Arrays Basics
git commit -m "📝 Day 1: Arrays Basics"
### ✅ Summary:
- Topics to Cover

1.Array Traversal
Visiting each element one by one.
Time Complexity: O(n)

2.Insertion in Arrays
Add element at:
End → O(1) (if space available)
Start / Middle → O(n) (need shifting)

3.Deletion in Arrays
Remove element at:
End → O(1)
Start / Middle → O(n) (need shifting)

4.Searching
Linear Search → Check each element, O(n).
Binary Search → Only for sorted arrays, O(log n).

### 🔗 Problems:
1.Traversal (Java)
public class ArrayTraversal {
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}

2.Linear Search (Java)
public class LinearSearch {
    public static int search(int[] arr, int key) {
        for (int i = 0; i < arr.length; i++) {
            if (arr[i] == key) return i;
        }
        return -1;
    }
    
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};
        int key = 30;
        int result = search(arr, key);
        System.out.println(result == -1 ? "Not Found" : "Found at index " + result);
    }
}

3. Binary Search (Java)
import java.util.Arrays;

public class BinarySearchExample {
    public static int binarySearch(int[] arr, int key) {
        int left = 0, right = arr.length - 1;
        while (left <= right) {
            int mid = left + (right - left) / 2;
            if (arr[mid] == key) return mid;
            if (arr[mid] < key) left = mid + 1;
            else right = mid - 1;
        }
        return -1;
    }
    
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};
        Arrays.sort(arr);
        int key = 40;
        int result = binarySearch(arr, key);
        System.out.println(result == -1 ? "Not Found" : "Found at index " + result);
    }
}