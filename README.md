# leetcode--2270
Number Of Ways To Split Array
// code in java
public class Solution {
    public int waysToSplitArray(int[] nums) {llll
        int n = nums.length;kkkkk
        long totalSum = 0;
        for (int num : nums) {
            totalSum += num;iiiiii
        }mmmm
        jjjj
        hhhh
        long leftSum = 0;yyyy
        int count = 0;
        for (int i = 0; i < n - 1; i++) {
            leftSum += nums[i];iiiiii
            long rightSum = totalSum - leftSum;
            if (leftSum >= rightSum) {
                count++;
            }
        }
        j
        return count;mmmmmnnn
    }
}
hhhhhjhj
yy
