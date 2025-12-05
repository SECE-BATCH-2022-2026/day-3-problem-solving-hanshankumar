import java.util.*;

class Main
{
	public static void main(String args[])
	{
		Scanner sc=new Scanner(System.in);
		String s1=sc.nextLine();
		String s2=sc.nextLine();
		int count=UserMainCode.countOccurance(s1,s2);
		System.out.println(count);
	}
}
class UserMainCode
{
	public static int countOccurance(String s1,String s2)
	{
		int count=0;
		int a=s2.length();
		
		for(int i=0;i<=s1.length()-a;i++)
		{
			if(s1.substring(i,i+a).equals(s2) )count++;
		}
		
		return count;
		
        
    }
	
}