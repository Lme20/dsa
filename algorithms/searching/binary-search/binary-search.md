# BINARY SEARCH - Find a target value in a sorted array

*Used to find a specific value in a sorted sequence*

*Repeatedly divides the search space in half until the target value is found*

*Commonly used in sorted arrays or sorted lists*

*You should count the index not the value of the elements!*



## Steps

Step 1: 
- Start with the entire sorted sequence.

Step 2:
- Calculate the middle index of the current search space. (not the elemenet value!)
left + right % 2

Step 3:
- Compare the middle element with the target value.

If the middle element is equal to the target value, return its index.
If the middle element is greater than the target value, repeat the process on the left half of the sequence.
If the middle element is less than the target value, repeat the process on the right half of the sequence.

*NOTE: UPDATE middle element all the time! if search left then -1, if search right then +1*
Step 4:
- Continue dividing the search space in half until the target value is found or the search space is empty.

### Calculating values

Middle index is calculated using the formula: `mid = (low + high) / 2`, where `low` and `high` represent the indices of the current search space.

## Pseudocode


## Asymptotic complexity: 

- Time complexity:
O(log n) worst-case where n is the size of the sorted sequence.

- Space complexity: 
O(1) worst-case 
Only requires a constant amount of additional space for storing values. 
