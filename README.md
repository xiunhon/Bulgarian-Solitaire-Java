# Bulgarian Solitaire
Java Projects
1/ Project ArrayList - Bulgarian Solitaire
Assignment

You will use only ArrayLists to write this program. This means that you cannot use arrays.
In this assignment, you will model the game of Bulgarian Solitaire.
The game starts with 45 cards. (They need not be playing cards. Unmarked index cards work just as well.)
Randomly divide them into some number of piles of random size.
For example, you might start with piles of size 20, 5, 1, 9, and 10.
In each round, you take one card from each pile, forming a new pile with these cards.
For example, the sample starting configuration would be transformed into piles of size 19, 4, 8, 9, and 5.
The solitaire is over when the piles have size 1, 2, 3, 4, 5, 6, 7, 8, and 9, in some order. (It can be shown that you always end up with such a configuration.)
In your program, produce a random starting configuration and print it.
Then keep applying the solitaire step and print the result.
Stop when the solitaire final configuration is reached.
There is more than one way to approach the initial number of piles. One way would be to be prompt the user for the initial number of piles. For two points of extra credit, prompt the user to enter an integer in a set range (ex. 2-9) and create that many piles with a random number of cards in each pile. Make sure that you validate the user's input so that a valid integer is entered in that range. You can use the CheckInput code on the code page for validation.
Sample Output
        	The initial piles are:
			30 7 8
			The new piles are:
			29 6 7 3
			The new piles are:
			28 5 6 2 4
			The new piles are:
			27 4 5 1 3 5
			The new piles are:
			26 3 4 2 4 6
			The new piles are:
			25 2 3 1 3 5 6
			The new piles are:
			24 1 2 2 4 5 7
			The new piles are:
			23 1 1 3 4 6 7
			The new piles are:
			22 2 3 5 6 7
			The new piles are:
			21 1 2 4 5 6 6
			The new piles are:
			20 1 3 4 5 5 7
			The new piles are:
			19 2 3 4 4 6 7
			The new piles are:
			18 1 2 3 3 5 6 7
			The new piles are:
			17 1 2 2 4 5 6 8
			The new piles are:
			16 1 1 3 4 5 7 8
			The new piles are:
			15 2 3 4 6 7 8
			The new piles are:
			14 1 2 3 5 6 7 7
			The new piles are:
			13 1 2 4 5 6 6 8
			The new piles are:
			12 1 3 4 5 5 7 8
			The new piles are:
			11 2 3 4 4 6 7 8
			The new piles are:
			10 1 2 3 3 5 6 7 8
			The new piles are:
			9 1 2 2 4 5 6 7 9
			The new piles are:
			8 1 1 3 4 5 6 8 9
			The new piles are:
			7 2 3 4 5 7 8 9
			The new piles are:
			6 1 2 3 4 6 7 8 8
			The new piles are:
			5 1 2 3 5 6 7 7 9
			The new piles are:
			4 1 2 4 5 6 6 8 9
			The new piles are:
			3 1 3 4 5 5 7 8 9
			The new piles are:
			2 2 3 4 4 6 7 8 9
			The new piles are:
			1 1 2 3 3 5 6 7 8 9
			The new piles are:
			1 2 2 4 5 6 7 8 10
			The new piles are:
			1 1 3 4 5 6 7 9 9
			The new piles are:
			2 3 4 5 6 8 8 9
			The new piles are:
			1 2 3 4 5 7 7 8 8
			The new piles are:
			1 2 3 4 6 6 7 7 9
			The new piles are:
			1 2 3 5 5 6 6 8 9
			The new piles are:
			1 2 4 4 5 5 7 8 9
			The new piles are:
			1 3 3 4 4 6 7 8 9
			The new piles are:
			2 2 3 3 5 6 7 8 9
			The new piles are:
			1 1 2 2 4 5 6 7 8 9
			The new piles are:
			1 1 3 4 5 6 7 8 10
			The new piles are:
			2 3 4 5 6 7 9 9
			The new piles are:
			1 2 3 4 5 6 8 8 8
			The new piles are:
			1 2 3 4 5 7 7 7 9
			The new piles are:
			1 2 3 4 6 6 6 8 9
			The new piles are:
			1 2 3 5 5 5 7 8 9
			The new piles are:
			1 2 4 4 4 6 7 8 9
			The new piles are:
			1 3 3 3 5 6 7 8 9
			The new piles are:
			2 2 2 4 5 6 7 8 9
			The new piles are:
			1 1 1 3 4 5 6 7 8 9
			The new piles are:
			2 3 4 5 6 7 8 10
			The new piles are:
			1 2 3 4 5 6 7 9 8
Press any key to continue . . .
