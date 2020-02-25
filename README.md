# COMPAREFILES
COMPARES DIFFERENT FILES
#include <iostream>
#include <fstream>
#include <string>

using namespace std;

int main ()
{
	/*
	ofstream file1("a.txt");
	ofstream file2("b.txt");
	ofstream file3("c.txt");
	if (!file1)
	{
		// Print an error and exit
		cerr << "Uh oh,a.txt could not be opened for writing!" << endl;
		exit(1);
	}

	// We'll write two lines into this file
	file1 << "This is line 1" << endl;
	file1 << "This is line 2" << endl;

	if (!file2)
	{
		// Print an error and exit
		cerr << "Uh oh, b.txt could not be opened for writing!" << endl;
		exit(1);
	}

	// We'll write two lines into this file
	file2 << "This is line 1" << endl;
	file2 << "This is line 2" << endl;

	if (!file3)
	{
		// Print an error and exit
		cerr << "Uh oh, b.txt could not be opened for writing!" << endl;
		exit(1);
	}

	// We'll write two lines into this file
	file3 << "This is line 1" << endl;
	file3 << "This is line 2" << endl;
	*/

	ifstream firstfile("a.txt");
	ifstream secondfile("b.txt");
	ifstream thirdfile("c.txt");

	if (!firstfile)
	{
		// Print an error and exit
		cerr << "Uh oh, a.txt could not be opened for writing!" << endl;
		exit(1);
	}

	if (!secondfile)
	{
		// Print an error and exit
		cerr << "Uh oh, b.txt could not be opened for writing!" << endl;
		exit(1);
	}

	if (!thirdfile)
	{
		// Print an error and exit
		cerr << "Uh oh, c.txt could not be opened for writing!" << endl;
		exit(1);
	}

	string Data1;
	string Data2;
	string Data3;
	if (firstfile)
	{
		
		//firstfile >> Data1;
		getline(firstfile, Data1);
		cout << Data1 << endl;

		
		//continue;
	}
	
	//string Data2;
	if (secondfile)
	{
		
		//secondfile >> Data2;
		getline(secondfile, Data2);
		cout << Data2 << endl;

		
		//continue;
	}

	//string Data3;
	if (thirdfile)
	{
		
		//thirdfile >> Data3;
		getline(thirdfile, Data3);
		cout << Data3 << endl;

		
		//continue;
	}
	

	if (Data1.compare(Data2) != 0)
		cout << "Data1 is not Data2" << '\n';
	else
		cout <<Data1<<  " is the same as "<< Data2 << endl;

	if (Data1.compare(Data3) != 0)
		cout << "Data1 is not Data3" << '\n';
	else
		cout << Data1 << " is the same as " << Data3 << endl;

	if (Data2.compare(Data3) != 0)
		cout << "Data2 is not Data3" << '\n';
	else
		cout << Data2 << " is the same as " << Data3 << endl;


		
	
}

