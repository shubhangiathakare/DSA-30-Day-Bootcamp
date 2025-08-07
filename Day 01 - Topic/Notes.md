# 📘 Day 01: 📘 Day 1: Time Complexity & Space Complexity

### ✅ Summary:
- 

### 🔗 Problems:
1. 
🔍 What You’ll Learn:
What is Time Complexity?

What is Space Complexity?

Understanding Big-O Notation

Analyzing code snippets

Common complexities (O(1), O(n), O(log n), O(n²), etc.)

Best, Average, Worst case scenarios

📚 Key Concepts
✅ Time Complexity:
Definition: It measures how the runtime of an algorithm changes with input size.

Notation: Common Big-O notations:

O(1) – Constant Time

O(n) – Linear Time

O(log n) – Logarithmic Time

O(n log n) – Linearithmic Time

O(n²) – Quadratic Time

✅ Space Complexity:
Definition: How much memory an algorithm uses with respect to the input size.

Includes variables, data structures, recursion stack, etc.

📌 Big-O Rules of Thumb
Drop constants: O(2n) → O(n)

Keep highest order term: O(n² + n) → O(n²)

Nested loops → multiply: two O(n) loops → O(n²)

Consecutive code → take the max: O(n) + O(n²) → O(n²)

🔍 Examples:
Example 1:
java

// O(n)
for (int i = 0; i < n; i++) {
    System.out.println(i);
}
Example 2:
java

// O(n²)
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        System.out.println(i + ", " + j);
    }
}
Example 3:
java

// O(log n)
int x = 1;
while (x < n) {
    x = x * 2;
}
🧠 Practice Now
📎 GFG Practice:
👉 GeeksforGeeks - Time Complexity MCQs

🛠 Mini Task:
Analyze the time and space complexity of 3 simple programs (loops, recursion, arrays).

Write them in a Day-01 folder (e.g., in Java or Python).
