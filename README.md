# Vending-Machine-Program
This program is for my assessment project to be summited in Code Lab 1, This program is for educational purpose only

#include <iostream>
#include <string>
using namespace std;

int main()
{
	int orderKey, quant, pickMon;
	char yepnah;
	string pick, figure;
	float coins = 0, settle, exchange;


	figure[1] = 20;

	do
	{
		cout << "\n\n    Welcome to Lucas Vending Machine! " << figure[1];
		cout << "                \n\n\n                    Table d'Hote";
		cout << "\n\n          1. Chocolates            \n          2. Chips       ";
		cout << "\n          3. Beverages        \n          4. Biscuits   ";
		cout << "\n          5. Waters            ";

		cout << "\n\n" << figure[1] << "\n Insert your money       :";
		cin >> settle;

		cout << "\n" << figure[1] << "\n Choose a category  (1-5)  ";
		cin >> orderKey;



		switch (orderKey)
		{
		case 1:
			pick = "Chocolates";
			cout << "                \n\n\n                    Table d'Hote";
			cout << "\n\n          1. Mars = 3.50 AED     \n          2. Hershey's = 2.50 AED      ";
			cout << "\n          3. Kitkat =  3.00 AED   \n          4. M&M's = 4.50 AED   ";
			cout << "\n          5. Galaxy = 5.50 AED           ";

			cout << endl << endl;

			cout << "\n" << figure[1] << "\n Choose a chocolate  (1-5):  ";
			cin >> pickMon;

			if (pickMon == 1)

			{
				 cout << "\nYour change will be " << settle - 3.50;
			}
			else if (pickMon == 2)
			{
				cout << "\nYour change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
			    cout << "\nYour change will be " << settle - 3.00;
			}
			else if (pickMon == 4)
			{
				cout << "\nYour change will be " << settle - 4.50;

			}
			else if (pickMon == 5)
			{
				 cout << "\nYour change will be " << settle - 5.50;
			}

			exchange = settle - pickMon;

			break;

		case 2:
			pick = "Chips";
			cout << "                \n\n\n                    Table d'Hote";
			cout << "\n\n          1. Oman Chips = 1.00 AED     \n          2. Lays Chips = 1.50 AED      ";
			cout << "\n          3. Pringles =  3.50 AED   \n          4. Cheetos = 1.50 AED   ";
			cout << "\n          5. Taxis = 3.00 AED           ";

			cout << endl << endl;

			cout << "\n" << figure[1] << "\n Choose a chip  (1-5):  ";
			cin >> pickMon;


			if (pickMon == 1)

			{
				cout << "\nYour change will be " << settle - 1.00;
			}
			else if (pickMon == 2)
			{
				cout << "\nYour change will be " << settle - 1.50;
			}
			else if (pickMon == 3)
			{
				cout << "\nYour change will be " << settle - 3.50;
			}
			else if (pickMon == 4)
			{
				cout << "\nYour change will be " << settle - 1.50;

			}
			else if (pickMon == 5)
			{
				cout << "\nYour change will be " << settle - 3.00;
			}

			exchange = settle - pickMon;

			break;

		case 3:
			pick = "Beverages";
			cout << "                \n\n\n                    Table d'Hote";
			cout << "\n\n          1. Rani = 1.50 AED     \n          2. Al Rawabi  = 2.50 AED      ";
			cout << "\n          3. Redbull =  5.50 AED   \n          4. Litpon = 3.50 AED   ";
			cout << "\n          5. Litchi = 2.00 AED           ";

			cout << endl << endl;

			cout << "\n" << figure[1] << "\n Choose a beverage  (1-5)";
			cin >> pickMon;


			if (pickMon == 1)

			{
				cout << "\nYour change will be " << settle - 1.50;
			}
			else if (pickMon == 2)
			{
				cout << "\nYour change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\nYour change will be " << settle - 5.50;
			}
			else if (pickMon == 4)
			{
				cout << "\nYour change will be " << settle - 3.50;

			}
			else if (pickMon == 5)
			{
				cout << "\nYour change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;

			break;

		case 4:
			pick = "Biscuits";
			cout << "                \n\n\n                    Table d'Hote";
			cout << "\n\n          1. Chips Ahoy = 5.50 AED     \n          2. Oreo  = 2.50 AED      ";
			cout << "\n          3. Dewberry =  4.00 AED   \n          4. Skyflakes = 1.50 AED   ";
			cout << "\n          5. Hansel = 2.00 AED           ";

			cout << endl << endl;

			cout << "\n" << figure[1] << "\n Choose a biscuit  (1-5)";
			cin >> pickMon;


			if (pickMon == 1)

			{
				cout << "\nYour change will be " << settle - 5.50;
			}
			else if (pickMon == 2)
			{
				cout << "\nYour change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "\nYour change will be " << settle - 4.00;
			}
			else if (pickMon == 4)
			{
				cout << "\nYour change will be " << settle - 1.50;

			}
			else if (pickMon == 5)
			{
				cout << "\nYour change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;

			break;

		case 5:
			pick = "Waters";
			cout << "                \n\n\n                    Table d'Hote";
			cout << "\n\n          1. Mai Dubai = 1.50 AED     \n          2. Arwa  = 2.50 AED      ";
			cout << "\n          3. Oasis =  1.00 AED   \n          4. Romana = 1.25 AED   ";
			cout << "\n          5. Al Ain = 2.00 AED           ";

			cout << endl << endl;

			cout << "\n" << figure[1] << "\n Choose a water  (1-5)";
			cin >> pickMon;


			if (pickMon == 1)

			{
				cout << "Your change will be " << settle - 1.50;
			}
			else if (pickMon == 2)
			{
				cout << "Your change will be " << settle - 2.50;
			}
			else if (pickMon == 3)
			{
				cout << "Your change will be " << settle - 1.00;
			}
			else if (pickMon == 4)
			{
				cout << "Your change will be " << settle - 1.25;

			}
			else if (pickMon == 5)
			{
				cout << "Your change will be " << settle - 2.00;
			}

			exchange = settle - pickMon;


			break;

		default:
			cout << "\n Invalid input, please try again!";
			break;
		}

		if (settle < coins)
		{
			cout << "\n           Sorry, you do not have enough money to proceed this transaction.  ";
			cout << " We have returned " << settle << " AED";
		}
		

		cout << "\n\n" << figure[1] << "Do you want to order again? (y/n):  ";
		cin >> yepnah;



	} while (yepnah == 'Y' || yepnah == 'y');

	cout << "\n\n   Thank you for your purchase, hope that you will buy again!";
}
