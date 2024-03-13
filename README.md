import java.util.*;
public class Main
{
	public static void main(String[] args)
	{
	    System.out.println("ENTER THE VALUE OF N");
	    Scanner sc = new Scanner(System.in);
	    int n = sc.nextInt();
	    System.out.println("ENTER THE VALUE OF ARRAY");
      int arr[]=new int[n];
      int a1=0;
      int b2=0;
      for(int i=0;i<n;i++)
      {
          arr[i]=sc.nextInt();
      }
      for(int i=0;i<n;i++)
      {
          if(arr[i]>a1)
          {
              b2=a1;
              a1=arr[i];
          }
          else if(arr[i]>b2&&arr[i]<a1)
          {
              b2=arr[i];
          }
      }
      System.out.println("1 st largest number is"+a1);
      System.out.println("2 nd largest number is"+b2);
	}
}
      
