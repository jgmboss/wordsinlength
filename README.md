import java.util.Scanner;

public class lengthofsaying
{
    public static void main (String [] arg) {
        int count = 1;
        Scanner input = new Scanner (System.in);
        System.out.println ("Please enter a saying");
        String saying = input.nextLine();

        while( saying.length() == 0)
        {
            System.out.println ("Please enter a saying");
            saying = input.nextLine();

        }

        for (int i = 0;i <= saying.length()-1;i++)
        {
            if (saying.charAt(i) == ' ' && saying.charAt(i+1)!=' ')
            {
                count++;
            }
        }
        System.out.println ("There are " + count + " words in that saying.");
    }

}   
