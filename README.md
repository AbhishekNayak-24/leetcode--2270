# leetcode--2270
Number Of Ways To Split Array
// code in java
public class Solution {
    public int waysToSplitArray(int[] nums) {llll
        int n = nums.length;kkkkk
        long totalSum = 0;
        for (int num : nums) {
            totalSum += num;
        }mmmm
        jjjj
        hhhh
        long leftSum = 0;
        int count = 0;
        for (int i = 0; i < n - 1; i++) {
            leftSum += nums[i];
            long rightSum = totalSum - leftSum;
            if (leftSum >= rightSum) {
                count++;
            }
        }
        
        return count;mmmmmnnnnnnnn
    }
}
