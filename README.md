# array
// Wonjin Choi
// CMSY-141/181 Computer Science I/Intro C++
// LAB_07 10/10/15
#include <iostream>
#include <string>
#include <iomanip>
#include <fstream>
using namespace std;




int main()

{
	const int SIZE = 10;
	int count;
	ofstream WriteDataFile;
	const int ROW = 10;
	const int COLU = 4;
	int stuff, quarters;
	string companies[SIZE] = { "MSFT" , "APPL","T","GPRO ", "IBM" , "GOOG" , "TSLA", "YHOO", "FB","WC" };
	int quaterly[ROW][COLU] = {		{53020.00, 80090.00, 23050.00 ,23500.00},
									{35070.00, 45230.00, 55030.00, 65000.00},
									{47090.00, 53070.00 ,44000.00, 45000.00},
									{27080.00, 27879.00, 93023.00, 56043.00},
									{45040.00,26004.00 ,27079.00, 28006.00},
									{31000.00, 32000.00, 33000.00, 34000.00},
									{23571.00 ,87345.00, 64205.00 ,29872.00},
									{42000.00, 43230.00, 47630.00, 23590.00},
									{12080.00, 34090.00, 43000.00, 25070.00},
									{27204.00, 87230.00, 29045.00, 24823.00,} };
	

	WriteDataFile.open("c:\temp\Data.txt");
	
	//Store values in the array.
		for (count = 0; count < SIZE; count++)
		companies[count] = count;
		
		// Open a file for output.
		WriteDataFile.open("c:\temp\Data.txt");
		
		// Write the array contents to the file.
		for (count = 0; count < SIZE; count++)
			WriteDataFile << companies[count] << endl;
		
		// Close the file.
		WriteDataFile.close();

	
	cout << endl; 
	cout << "Lab-07 Wonjin Choi" << endl; 
	system("Pause");
	return 0;
}

