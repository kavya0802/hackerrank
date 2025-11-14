import java.util.Scanner;

public class Solution {

    

   
    static boolean isAnagram(String a, String b) {
         a = a.toLowerCase();
        b = b.toLowerCase();

        if (a.length() != b.length()) return false;

        String tempB = b;

        for (int i = 0; i < a.length(); i++) {
            char ch = a.charAt(i);
            int index = tempB.indexOf(ch);
            if (index == -1) {
                return false;
            } else {
                tempB = tempB.substring(0, index) + tempB.substring(index + 1);
            }
        }

        return true;


    }

    public static void main(String[] args) {
    
        Scanner scan = new Scanner(System.in);
        String a = scan.next();
        String b = scan.next();
        scan.close();
        boolean ret = isAnagram(a, b);
        System.out.println( (ret) ? "Anagrams" : "Not Anagrams" );
    }
}
