import java.util.*;

/**@author
 * due date: 2021
 * 
 * Bulgarian Solitaire model using ArrayList
 * Each index of the ArrayList holds a pile of cards. The deck has 45 cards.
 * Prompt user's input for starting no. of piles
 * Generate random no. of cards into each pile, except the last one,
 * the last index holds the rest of the deck
 * Output the initial piles
 * Perform Solitaire step. Remove 1 card from each pile,
 * form a new pile from those removed cards
 * Print the result of each step
 * Keep doing that until the piles have size 1,2,3,4,5,6,7,8,9 in some order
 * 
 */
public class Solitaire 
{
	// simplify main() + print ArrayList in a desired format
	public static void printArray(String header, ArrayList<Integer> array)
	{
		System.out.println("     " + header);
		System.out.print("     ");
		for (Integer i : array)
		{
			System.out.print(i + " ");
		}
		System.out.println();
	}//printArrayList ends
	
	// isFinal method checks if the solitaire step reaches the last configuration
	public static boolean isFinal (ArrayList<Integer> list)
	{
	    // sort the list
	    ArrayList<Integer> sortedList = new ArrayList<Integer>(list);
	    Collections.sort(sortedList);
	    int countdown = sortedList.size()-1; // count from numofPiles
	    
	    // check if the sorted list is in the exact order 1 to 9
	    if (sortedList.size() == 9 && 
	    	sortedList.get(0) == 1 && 
	    	sortedList.get(sortedList.size()-1) == 9)
	    {
	    	for (int i=sortedList.size()-1; i>0; i--)
	    	{
	    		if (sortedList.get(i)-1 == sortedList.get(i-1))
	    		{
	    			countdown--; 
	    		}
	    	}
	    }
	    if (countdown == 0) // no pile left, condition is met
	    {
	    	return true;
	    }
	    return false;
	}// end of isFinal
	
	// Main Driver
	public static void main(String[] args) 
	{
		// use only ArrayList
		ArrayList<Integer> piles = new ArrayList<Integer>();
		Random rand = new Random();
				
		/* prompt the user for number of piles, 
		** range from 2 to 9 piles, use CheckInput to get the right one in the range
		*/
		System.out.println("Bulgarian Solitaire - Start!");
		System.out.println("How many piles would you like to start? (2 to 9 piles)");
		int numofPiles = CheckInput.getIntRange(2, 9);
				
		/* Generate random numbers to each pile */
		int deck = 45;
		int freePiles = numofPiles; //start from numofPiles, decrease by 1 each loop
				
		
		while (freePiles > 1)	// loop to add random cards to each pile, except the last one (freePiles = 1)
		{
			int pileSize = rand.nextInt(deck-freePiles) + 1; 	
		    // random size from 0 to 44, +1 make sure random size is not 0
			// make sure leave at least 1 card for other piles
			piles.add(pileSize);	// add to ArrayList
			deck = deck - pileSize;	// update the remained cards
			freePiles--;
		}//while loop ends
		piles.add(deck); // add the rest of the deck to the last input
				
		/* Output the initial piles */
		System.out.print("The initial piles are:");
		printArray("", piles);


		/* Soliatire step, take 1 card each pile, put them in a new pile */
		while (true)
		{
			int newPile = 0;
			for (int i = 0; i<piles.size(); i++)
			{
				piles.set(i, piles.get(i) - 1);	// take 1 card from each pile
		        newPile++;	
			}
			piles.add(newPile);	// form a new pile from removed cards
			
			// remove zero before printing the new piles
			piles.removeIf(n -> n == 0);
			numofPiles = piles.size();
			printArray("The new piles are:", piles); // print the result of each step

			// call isFinal, if true, exit while loop
			if (isFinal(piles) == true)
			{
				System.out.println("The final configuration is reached!!!");
				break;
			}
		}//while loop ends
		
	}//end of main
	
}//end of class
