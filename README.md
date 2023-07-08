import java.util.Scanner;

class Learn{
	
	public static void main(String[]ar) {
		
	   Scanner sc=new Scanner(System.in);
	   Learn obj=new Learn();
	   int player=0;
	   int robot=0;
	   System.out.println("enter the choclate you want multuple with 4");
		  
	  
	   int n=sc.nextInt();
	   int chilli=1;
	   int choclate=(4*n)+1;
	   System.out.println("there are totally "+choclate+" choclate and one chilli");
	   
	   choclate-=1;
	 System.out.println("your opponent starts the game and he took one choclate");
	   

	 while(choclate!=0) {
		   System.out.println("take one or two or three choclate as your choise");
		   player=sc.nextInt();
		   choclate-=player;
		   
		   
		   
		   if(player==1) {
			   choclate-=3;
			   robot=3;
			   
		   }else if(player==2) {
			   choclate-=2;
			   robot=2;
		   }
		   
		   
		   else if(player==3) {
			   choclate-=1;
			   robot=1;
		   }
		  System.out.println("your opponent took "+robot+" choclate");
		   System.out.println("the number of choclate remaining = "+choclate);
		   System.out.println("the chilli = "+chilli);
		  
	   }
	     System.out.println("you lose the game");
	}
}
	  
		

