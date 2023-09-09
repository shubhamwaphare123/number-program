package PracticeQuestion;

import java.util.Scanner;

public class rverseNum {
	
	public int rev(int n) {
		int rev=0;
		for(; n>0;n=n/10 ) {
			int last_dig = n%10;
			rev=rev*10+last_dig;
			
		}
//		System.out.println(rev);
		return(rev);
	}
	

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc = new Scanner(System.in);
		System.out.println("enter a number :-");
		int n = sc.nextInt();
		
		rverseNum r1= new rverseNum();
		int res = r1.rev( n);
		System.out.print(res);

	}

}
