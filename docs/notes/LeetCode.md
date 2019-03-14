# 演算法
[Leetcode ：167. Two Sum II - Input array is sorted (Easy)](https://leetcode.com/problems/two-sum/)
```
# O(n) time complexity
class Solution(object):
    def twoSum(self, nums, target):
        if len(nums) <= 1:
            return False
        buff_dict = {}
        for i in range(len(nums)):
            # find in dictionary O(1) time
            if nums[i] in buff_dict:
                return [buff_dict[nums[i]], i]
            else:
                buff_dict[target - nums[i]] = i
```
[Leetcode ：704. Binary Search (Easy)](https://leetcode.com/problems/binary-search/)
``` O(log n) time complexity
class Solution {
public:
    int search(vector<int>& nums, int target) {
        l , r = 0, len(r) - 1 
        while l <= r :
            mid = l + r 
            if target > num[mid] :
                l = mid + 1
            elif target < num[mid] :
                r = mid -1 
            else :
                return mid
        return -1
    }
};
```
[Leetcode ：371. Sum of Two Integers](https://leetcode.com/problems/sum-of-two-integers/)
* Calculate the sum of two integers a and b, but you are not allowed to use the operator + and - .
```
class Solution:
    def getSum(self, a, b):
        """
        :type a: int
        :type b: int
        :rtype: int
        """
        list = (a,b)
        return sum(list)
```
[Leetcode ：804. Jewels and Stones](https://leetcode.com/problems/jewels-and-stones/)
```
class Solution:
 def numJewelsInStones(self, J, S):
    return sum(map(J.count, S))
 def numJewelsInStones(self, J, S):
    return sum(map(S.count, J))   
 sum( map(lambda x:s.count(x) ,j))
 def numJewelsInStones(self, J, S):
    return sum(s in J for s in S) 

```
map()