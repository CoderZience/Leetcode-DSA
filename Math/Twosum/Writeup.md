## Description

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.

## Walkthrough
----------------------



```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        hashmap = {} 
        for i in range(len(nums)):
            answer = target - nums[i]                                     
            if answer in hashmap:
                return[i,hashmap[answer]]
            hashmap[nums[i]] = i 
            
```
