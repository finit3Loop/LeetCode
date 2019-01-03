//my solution
class Solution {
    public String toLowerCase(String str) {
        
        char[] chars = new char[str.length()];
		chars = str.toCharArray();
        
        for (int i = 0; i < str.length(); i++) {

			int ascii = (int) chars[i];
            
            if (ascii <= 90 && ascii >= 65) {
				System.out.println((char) (ascii + 32));
				chars[i] = ((char) (ascii + 32));
				//System.out.println(chars[i]);
			}

		}
		str = chars.toString();
		return str ;
        
    }
}

//MainClass provided by leetcode to test
public class MainClass {
    public static String stringToString(String input) {
        return JsonArray.readFrom("[" + input + "]").get(0).asString();
    }
    
    public static void main(String[] args) throws IOException {
        BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
        String line;
        while ((line = in.readLine()) != null) {
            String str = stringToString(line);
            
            String ret = new Solution().toLowerCase(str);
            
            String out = (ret);
            
            System.out.print(out);
        }
    }
}
