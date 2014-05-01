DICE-TEST-LAB---3--WEEK---11
============================

DICE TEST LAB #3  WEEK # 11


//  BY REINA OLARTE

//  DICE-TEST LAB# 3 - WEEK 11

import java.util.Scanner;

public class DiceTest 
{
	public static void main( String[]args)	
	{
	Scanner input = new Scanner(System.in);
// variables 
	
	int COMPNumber;
	
	int NUMBRolls;
	
	String Answer;
	
	boolean SIGA = true;
	
		while(SIGA)
			
		{
			
		System.out.println("What number of rolls  would you like to play: ");
		
		NUMBRolls = input.nextInt();
		
		Dice myDice = new Dice(NUMBRolls);

		COMPNumber = myDice.Value();
		
		System.out.printf("The Number that was rolled from the dice was : %d\n\n", COMPNumber);
		
		System.out.println("Do you want to continue?( yes = Y or no = N): ");
		
		Answer= input.next();
		
			if(Answer.toUpperCase().startsWith("N"))
			{
				SIGA = false;
			}
		}
	}
}
