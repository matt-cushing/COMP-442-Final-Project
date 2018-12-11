# COMP-442-Final-Project

//This program allows the user to input the cost of the meal, tax, tips, and or splits the bill between party members.

import java.util.Scanner;

public class Split {

	public static void main(String[] args) {
		
		
		//Declare variables. 
		Scanner scanner = new Scanner(System.in);
		double mealCost;
		double stateTax;
		double tax;
		double tip;
		double totalCost;
		double goodService;
		int partyMember;
		double split;
	
					
		//Ask the user for meal cost.
		System.out.println("Enter the cost of the meal: ");
		mealCost = scanner.nextDouble();
		
		//Ask the user for the state tax.
		System.out.println("Enter the state tax: ");
		stateTax = scanner.nextDouble();
		
		//Calculates the tax and the total cost. 
		tax = mealCost * stateTax;
		totalCost = mealCost + tax;
		System.out.println("Meal Tax: $" + tax );
		System.out.println("Total Cost of Meal: $" + totalCost);	
		
		//Ask the user for the tip, calculate the tip, and prints it out.
		System.out.println("Enter amount to tip: ");
		tip = scanner.nextDouble();
		goodService = totalCost * tip;
		System.out.println("Tip Amount: $" + goodService);
		
		//Ask the user amount of people in party.
		System.out.println("How many people in your party? ");
		partyMember = scanner.nextInt();
		split = totalCost / partyMember;
		System.out.println("Each person will pay: $" + split);
		
		
		
		
		
		
		
	}

}
