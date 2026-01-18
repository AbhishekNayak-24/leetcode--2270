# leetcode--2270
Number Of Ways To Split Array
// code in java
public class Solution {
    public int waysToSplitArray(int[] nums) {
        int n = nums.length;
        long totalSum = 0;
        for (int num : nums) {
            totalSum += num;
        }mmmm
        jjjj
        
        long leftSum = 0;
        int count = 0;
        for (int i = 0; i < n - 1; i++) {
            leftSum += nums[i];
            long rightSum = totalSum - leftSum;
            if (leftSum >= rightSum) {
                count++;
            }
        }
        kkkkk
        return count;
    }
}
