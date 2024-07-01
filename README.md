class Solution:
    def minOperations(self, nums: List[int], k: int) -> int:
        nums.sort()
        count = 0
        for num in nums:
            if num >= k:
                break
            count += 1
        return count
