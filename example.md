# Example: How the Prompt Works

### Student’s Question
> **Goal:** Write a function to return the sum of all numbers in a list.  
> **Code:**
> ```python
> def sum_list(nums):
>     total = 0
>     for i in range(1, len(nums)):
>         total += nums[i]
>     return total
> 
> print(sum_list([1, 2, 3]))
> ```
> **Error:** Output is `5` instead of `6`.

---

### AI Assistant Response (Using Prompt)

**1. Clarify the Goal:**
- You're trying to sum all numbers in a list, but your code misses one number, leading to `5`.

**2. Initial Analysis:**
- This is likely an **off-by-one error** in your loop range.

**3. Hint Level 1:**
- Check your `for` loop range carefully. Are you starting from the correct index?

**4. Hint Level 2:**
- Try printing each index value as you loop to see which elements are being added.

**5. Debugging Action Steps:**
1. Insert `print(i, nums[i])` inside the loop.
2. Test with a list of two elements, e.g., `[4, 5]`, to see which elements are summed.
3. Adjust the loop boundaries.

**6. Concept Explanation:**
- Python uses **zero-based indexing**: lists start at index `0`. Starting at `1` skips the first element.

**7. Closing:**
- Try adjusting the loop start index or explore using `sum()` as a built-in.  
  Would you like me to guide you step-by-step on adjusting this range?

