import java.util.Scanner;
import java.util.List;
import java.util.ArrayList;
import java.util.Arrays;

class ThreeSum {

  // Time complexity: O(n^2)
  private static List<Integer[]> findThreeSum_Sorting(int[] nums, int target) {
    List<Integer[]> result = new ArrayList<>();
    Arrays.sort(nums);
    for (int i = 0; i < nums.length; i++) {
      int left = i + 1;
      int right = nums.length - 1;
      while (left < right) {
        if (nums[i] + nums[left] + nums[right] == target) {
          result.add(new Integer[] { nums[i], nums[left], nums[right] });
          left++;
          right--;
        } else if (nums[i] + nums[left] + nums[right] < target) {
          left++;
        } else {
          right--;
        }
      }
    }
    return result;
  }
}
