package 예제2;
import java.util.Scanner;

public class openChallenge {
	public static void main(String[]args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("가위 바위 보 게임입니다. 가위, 바위, 보 중에서 입력하세요");
		System.out.print("철수 >>");
		String var1 = sc.next();	//var1=철수
		
		System.out.print("영희 >>");
		String var2 = sc.next();	//var2=영희
		
		if(var1.equals("가위")) {
			if(var2.equals("바위"))
				System.out.println("영희가 이겼습니다");
			else if(var2.equals("보"))
				System.out.println("철수가 이겼습니다");
		}
		else if(var1.equals("바위")) {
			if(var2.equals("가위"))
				System.out.println("철수가 이겼습니다");
			else if(var2.equals("보"))
				System.out.println("영희가 이겼습니다");
		}
		else if(var1.equals("보")) {
			if(var2.equals("가위"))
				System.out.println("영희가 이겼습니다");
			else if(var2.equals("바위"))
				System.out.println("철수가 이겼습니다");
		}		
		else
			System.out.println("비겼습니다");
			
		sc.close();	
	 }
}
