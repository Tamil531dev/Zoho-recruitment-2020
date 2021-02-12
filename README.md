import java.util.Scanner;

public class Zoho
{
	public static void main(String[] args)
	{
		Scanner scan = new Scanner(System.in);
		String s = scan.next();
		for (int i = 0; i < s.length(); i++)
		{
			int n = s.length()/2;
			for (int j = 0; j < s.length()-i; j++)
				System.out.print(" ");
			for (int j = 0; j <= i; j++)
			{
				System.out.print(s.charAt(n));
				n++;
				if(n==s.length())
					n=0;
			}
			System.out.println();
		}
		scan.close();
	}
}
