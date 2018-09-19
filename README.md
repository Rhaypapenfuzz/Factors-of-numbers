# Factors-of-numbers
//Ask user for an integer input and then print respective factors of that number
#include <iostream>
#include <iomanip>
#include <list>
using namespace std;

//functions
int numFactors(int);

int main()
{
	int userInteger;
	cout << "Enter any integer: ";
	cin >> userInteger;
	//for(int g = 0;g<5;g++)
	
	numFactors(userInteger);
	
	system("pause");
	return 0;
}
	int numFactors(int userInteger) 
	{
		list<int>factors{};
		int factor;
		for (int i = 1; i <= userInteger; i++)
			if (userInteger % i==0)
				//factors.insert(i);
				factors.push_back(i); 
		for (auto v : factors)
		cout << v << "\n";

		return 5;
}
