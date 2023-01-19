
#include <iostream>
using namespace std;

bool isNumber(string s)

{

	for (int i = 0; i < s.length(); i++)

		if (isdigit(s[i]) == false)

			return false;

	return true;

}

int main() {

	string myname;

	do {

		cout << "Enter my name" << endl;

		cin >> myname;

		if (isNumber(myname)) { cout << "That is a number! "; };

	} while (myname != "Stanislavs");

	return 0;

}
