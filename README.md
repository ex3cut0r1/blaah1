# blaah1package Homework_3;
import java.util.Scanner;
import java.util.Random;
public class EziTura {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		Random rand = new Random();
		String[] EziTura = {"ezi", "ezi","ezi", "tura","tura", "tura"};	
		
		
    String temp1 = EziTura[rand.nextInt(6)] ;
    String foor1 = null ;
	int counter1 = 0;
	int counter2 = 0;
	String Start;
	do {
		System.out.println("Type in 'Start' to throll the coin or 'Close' to close the program");
		Start = sc.nextLine();
	}while(!Start.equals("Start") && !Start.equals("Close")); {
		
		if(Start.equals("Start")) {
			
			for(int i = 0; ;i++) {
				do {
					System.out.println("Ezi");
					if(!EziTura[rand.nextInt(6)].equals("ezi")) {
						
					if( foor1 == temp1 ) {
						counter1++;
					}
					else {counter1 = 0;}
					} foor1 = EziTura[rand.nextInt(6)];
					
						}while(!EziTura[rand.nextInt(6)].equals("ezi"));
				do {
					System.out.println("Tura");
					if(!EziTura[rand.nextInt(6)].equals("tura")) {
						
					if (foor1 == temp1) {
						counter2++;
					}
					else { counter2 = 0;}
					}foor1 = EziTura[rand.nextInt(6)];
					
						}while(!EziTura[rand.nextInt(6)].equals("tura"));
				if(counter1 == 3) {
					System.out.println("Three Consecutive Ezi's");
					break;
				}
				if(counter2 == 3) {
					System.out.println("Three Consecutive Tura's");
				}
			}
	}
	if(Start.equals("Close")); {
		System.out.println("See you next time!");
		
	}
		
			
	}
}
}
