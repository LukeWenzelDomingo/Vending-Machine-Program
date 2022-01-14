# Vending-Machine-Program
This program is for my assessment project to be summited in Code Lab 1, This program is for educational purpose only
        #include <iostream>
        #include <string>
        #include<stdio.h>

        using namespace std;

        int main()
{
	// Declaring the variable names to be used in the vending machine
	int orderKey, quant, pickMon;
	char yepnah;
	string pick, figure[1];
	float coins = 0, settle, exchange;

	figure[0];

	do
	{
		// Setting the menu for every category of my vending machine
		// The couts prints the box to be shown on the result screen
		cout << " \n                  |********************************************************|";
		cout << " \n                  |            Welcome to Lucas Vending Machine!           |" << figure[0];
		cout << " \n                  |--------------------------------------------------------|";
		cout << " \n                  |                     Table d'Hote                       |";
		cout << " \n                  |--------------------------------------------------------|";
		cout << " \n                  |         1. Candies        |       2. Chips             |";
		cout << " \n                  |--------------------------------------------------------|";
		cout << " \n                  |         3. Beverages      |       4. Biscuits          |";
		cout << " \n                  |--------------------------------------------------------|";
		cout << " \n                  |                      5. Water                          |";
		cout << " \n                  |                                                        |";
		cout << " \n                  **********************************************************";

		// This will ask the user to enter his/her money amount
		cout << "\n\n" << figure[0] << "\n                    Insert your money       :"; 
		cin >> settle;

		// This will ask the user to pick a category of food they want to eat
		cout << "\n" << figure[0] << "\n                    Choose a category  (1-5)  ";
		cin >> orderKey;


		// The switch function will switch between the categories written on the first board menu
		switch (orderKey)
		{
		case 1:
			// If the user pick the number 1 this will print the candy menu box
			system("CLS"); //Prints to another page
			pick = "Chocolates";
			cout << "\n                 |******************************************************|";
			cout << "\n                 |                     Table d'Hote                     |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |     1. Mars = 3.50 AED    |  2. Skittles  = 2.50 AED |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |     3. Kitkat = 3.00 AED  |  4. M&M's = 4.50 AED     |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |           5. Haribo's Gummy Bear = 5.50 AED          |";
			cout << "\n                 ********************************************************";

			cout << endl << endl; // spaces
			// This will ask the user to choose a candies in the menu
			cout << "\n" << figure[0] << "\n                    Choose a chocolate  (1-5):  " << " ";
			cin >> pickMon;

			// Condition for the changes in every candy in the menu and prints them in the result screen
			if (pickMon == 1)

			{
				cout << "\n                    Your change will be " << settle - 3.50;
			}
			else if (pickMon == 2)
			{
				cout << "\n                    Your change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\n                    Your change will be " << settle - 3.00;
			}
			else if (pickMon == 4)
			{
				cout << "\n                    Your change will be " << settle - 4.50;

			}
			else if (pickMon == 5)
			{
				cout << "\n                    Your change will be " << settle - 5.50;
			}

			exchange = settle - pickMon;
			
			break;

		case 2:
			// If the user pick the number 2 this will print the chips menu box
			system("CLS"); // prints to another page
			pick = "Chips";
			cout << "\n                 |*******************************************************|";
			cout << "\n                 |                     Table d'Hote                      |";
			cout << "\n                 |-------------------------------------------------------|";
			cout << "\n                 |  1. Oman Chips = 1.00 AED |  2. Lays Chips = 1.50 AED |";
			cout << "\n                 |-------------------------------------------------------|";
			cout << "\n                 |  3. Pringles = 3.50 AED   |  4. Cheetos = 2.00 AED    |";
			cout << "\n                 |-------------------------------------------------------|";
			cout << "\n                 |                  5. Taxis = 5.50 AED                  |";
			cout << "\n                 *********************************************************";

			cout << endl << endl; //spaces
			// This will ask the user to choose a chip in the menu
			cout << "\n" << figure[0] << "\n                    Choose a chip  (1-5):  ";
			cin >> pickMon;

			// Condition for the changes in every chips in the menu and prints them in the result screen
			if (pickMon == 1)

			{
				cout << "\n                    Your change will be " << settle - 1.00;
			}
			else if (pickMon == 2)
			{
				cout << "\n                    Your change will be " << settle - 1.50;
			}
			else if (pickMon == 3)
			{
				cout << "\n                    Your change will be " << settle - 3.50;
			}
			else if (pickMon == 4)
			{
				cout << "\n                    Your change will be " << settle - 1.50;

			}
			else if (pickMon == 5)
			{
				cout << "\n                    Your change will be " << settle - 3.00;
			}

			exchange = settle - pickMon;

			break;

		case 3:
			// If the user pick the number 3 this will print the beverages menu box
			system("CLS"); // prints to another page
			pick = "Beverages";
			cout << "\n                 |******************************************************|";
			cout << "\n                 |                     Table d'Hote                     |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |     1. Rani = 1.50 AED    |  2. Al Rawabi = 2.50 AED |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |     3. Redbull = 5.50 AED |  4. Lipton = 3.50 AED    |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |                 5. Litchi = 2.00 AED                 |";
			cout << "\n                 ********************************************************";


			cout << endl << endl;
			// This will ask the user to choose a beverage in the menu
			cout << "\n" << figure[0] << "\n                    Choose a beverage  (1-5)";
			cin >> pickMon;

			// Condition for the changes in every beverages in the menu and prints them in the result screen
			if (pickMon == 1)

			{
				cout << "\n                    Your change will be " << settle - 1.50;
			}
			else if (pickMon == 2)
			{
				cout << "\n                    Your change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\n                    Your change will be " << settle - 5.50;
			}
			else if (pickMon == 4)
			{
				cout << "\n                    Your change will be " << settle - 3.50;

			}
			else if (pickMon == 5)
			{ 
				cout << "\n                    Your change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;

			break;

		case 4:
			// If the user pick the number 4 this will print the biscuits menu box
			system("CLS"); // prints to another page
			pick = "Biscuits";
			cout << "\n                 |******************************************************|";
			cout << "\n                 |                     Table d'Hote                     |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |  1. Chips Ahoy = 5.50 AED |  2. Oreo = 2.50 AED      |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |  3. Dewberry = 4.00 AED   |  4. Skyflakes = 1.50 AED |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |                 5. Hansel = 2.00 AED                 |";
			cout << "\n                 ********************************************************";


			cout << endl << endl;
			// This will ask the user to choose a biscuit in the menu
			cout << "\n" << figure[0] << "\n                    Choose a biscuit  (1-5)";
			cin >> pickMon;

			// Condition for the changes in every biscuits in the menu and prints them in the result screen
			if (pickMon == 1)

			{
				cout << "\n                    Your change will be " << settle - 5.50;
			}
			else if (pickMon == 2)
			{
				cout << "\n                    Your change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\n                    Your change will be " << settle - 4.00;
			}
			else if (pickMon == 4)
			{
				cout << "\n                    Your change will be " << settle - 1.50;

			}
			else if (pickMon == 5)
			{
				cout << "\n                    Your change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;

			break;

		case 5:
			// If the user pick the number 5 this will print the water menu box
			system("CLS"); // prints to another page
			pick = "Waters";
			cout << "\n                 |******************************************************|";
			cout << "\n                 |                     Table d'Hote                     |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |   1. Mai Dubai = 1.50 AED |     2. Arwa = 2.50 AED   |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |   3. Oasis = 1.00 AED     |     4. Romana = 1.25 AED |";
			cout << "\n                 |------------------------------------------------------|";
			cout << "\n                 |                 5. Al Ain = 2.00 AED                 |";
			cout << "\n                 ********************************************************";


			cout << endl << endl;
			// This will ask the user to choose a water in the menu
			cout << "\n" << figure[0] << "\n                    Choose a water  (1-5)";
			cin >> pickMon;

			// Condition for the changes in every water in the menu and prints them in the result screen
			if (pickMon == 1)

			{
				cout << "\n                    Your change will be " << settle - 1.50;
			}
			else if (pickMon == 2)
			{
				cout << "\n                    Your change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\n                    Your change will be " << settle - 1.00;
			}
			else if (pickMon == 4)
			{
				cout << "\n                    Your change will be " << settle - 1.25;

			}
			else if (pickMon == 5)
			{
				cout << "\n                    Your change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;


			break;

		default:
			// Prints if the user enter a higher and lower number than 1-5
			cout << "\n                         Invalid input, please try again!";
			break;
		}
		// Condition is the user doesn't have enough money to buy the item
		if (settle < coins)
		{
			cout << "\n                         Sorry, you do not have enough money to proceed this transaction.  ";
			cout << "\n                         We have returned " << settle << " AED";
		}

		// Ask the user if they want to order another food to partner the food they ordered
		cout << endl << endl;// Spaces

		cout << "\n\n" << figure[0] << "\n                    Do you want to order again to partner the one you just ordered? (y/n):  ";
		cin >> yepnah;


    // Loops the vending machine if the user entered y/Y
	} while (yepnah == 'Y' || yepnah == 'y');
	// This will print if the user enter N/n 
	cout << "\n\n                             Thank you for your purchase, hope that you will buy again!";
}
