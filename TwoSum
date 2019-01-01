//Solution
class Solution {
    public int[] twoSum(int[] nums, int target) {
        
        int[] solution = new int[2];
        for(int n=0; n<nums.length; n++)
        {
            
            int int1 = nums[n];
            for(int m=0; m<nums.length; m++)
            {
                int int2 = nums[m];
                    
                    //System.out.println("int1 = "+int1);
                    //System.out.println("int2 = "+int2);
                    
                    if (int1+int2 == target && n != m)
                    {
                      //  System.out.println("n = "+n);
                       // System.out.println("m = "+m);
                        
                        solution[0] = m;
                        solution[1] = n;
                    }
                
            }
            
        }
     
        return solution;
    }
}

//LeetCode running code for Two Sum
public class MainClass {
    public static int[] stringToIntegerArray(String input) {
        input = input.trim();
        input = input.substring(1, input.length() - 1);
        if (input.length() == 0) {
          return new int[0];
        }
    
        String[] parts = input.split(",");
        int[] output = new int[parts.length];
        for(int index = 0; index < parts.length; index++) {
            String part = parts[index].trim();
            output[index] = Integer.parseInt(part);
        }
        return output;
    }
    
    public static String integerArrayToString(int[] nums, int length) {
        if (length == 0) {
            return "[]";
        }
    
        String result = "";
        for(int index = 0; index < length; index++) {
            int number = nums[index];
            result += Integer.toString(number) + ", ";
        }
        return "[" + result.substring(0, result.length() - 2) + "]";
    }
    
    public static String integerArrayToString(int[] nums) {
        return integerArrayToString(nums, nums.length);
    }
    
    public static void main(String[] args) throws IOException {
        BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
        String line;
        while ((line = in.readLine()) != null) {
            int[] nums = stringToIntegerArray(line);
            line = in.readLine();
            int target = Integer.parseInt(line);
            
            int[] ret = new Solution().twoSum(nums, target);
            
            String out = integerArrayToString(ret);
            
            System.out.print(out);
        }
    }
}
