leetcode-01

class Solution {
    public int[] twoSum(int[] nums, int target) {
        int l = nums.length;
        int[] ans = new int[2];
        int i,j;
        for(i = 0; i < l - 1; i++)
            for(j = i + 1; j < l; j++) {
                if(nums[i] + nums[j] == target) {
                    ans[0] = i;
                    ans[1] = j;
                }
            }
        return ans;
    }
}
