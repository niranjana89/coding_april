/**

Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order.

You must write an algorithm with O(log n) runtime complexity.

 

Example 1:

Input: nums = [1,3,5,6], target = 5
Output: 2
Example 2:

Input: nums = [1,3,5,6], target = 2
Output: 1
Example 3:

Input: nums = [1,3,5,6], target = 7
Output: 4
 

Constraints:

1 <= nums.length <= 104
-104 <= nums[i] <= 104
nums contains distinct values sorted in ascending order.
-104 <= target <= 104



**/

//https://leetcode.com/problems/search-insert-position/description/?source=submission-noac

class Solution {
    public int searchInsert(int[] nums, int target) {
    
        int n = nums.length;
        int l= 0;
        int r = nums.length-1;
        int ans = n;
        while( l <= r){
            int mid = (l+r)/2;
            if(nums[mid] >= target){
                ans = mid;
                r = mid-1;
            }else{
                l= mid+1;
            }


        }
        return ans;

    }

    public int searchFind(int l, int r, int target, int[] a){

        
       if( r < 0 || l > a.length-1 || l==r){

        if( r == 0 ){
            
        }
        //to the left -> either at 0 or 1 

       //to the right -> either at a.length-1  or a.length-2

       }
       
        int i = (l+r)/2;
        if(a[i] == target){
            return i;
        }else if( a[i] < target){
            return searchFind(i+1, r, target, a);
        }else {
            return searchFind(l, i-1 , target, a);
        }

    }
}
