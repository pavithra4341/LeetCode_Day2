# 📌 LeetCode 2: Add Two Numbers

## Problem
You are given two **non-empty linked lists** representing two non-negative integers.
The digits are stored in **reverse order**, and each node contains a single digit.

Add the two numbers and return it as a linked list.

### Example 1
**Input:** l1 =, l2 = [2,4,3][5,6,4]
**Output:**
**Explanation:** 342 + 465 = 807[7,0,8]

### Example 2
**Input:** l1 =, l2 = [0]
**Output:**[0]

### Constraints
- Nodes in each list: `1 to 100`
- `0 <= Node.val <= 9`

[🔗 Solve on LeetCode](https://leetcode.com/problems/add-two-numbers/)

---

## 💡 Approach
Same as manual addition with carry.

1. Use a `dummy` node to build the result list
2. `sum = l1.val + l2.val + carry`
3. `new_node = sum % 10`
4. `carry = sum / 10`
5. Move pointers. Loop until both lists and carry are 0

**Time:** `O(max(m,n))`
**Space:** `O(max(m,n))`



