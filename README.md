# WSQ14.cpp
e

/*
#WSQ14
Main: setprecision(num) << (numero o funcion) <<
By: Jorge Cervantes
#TC1017
Referencia: Cplusplus.com,. (2015). setprecision - C++ Reference. Retrieved 6 April 2015, from http://www.cplusplus.com/reference/iomanip/setprecision/
---------------------------------------------------------------------
*/

#include <iostream>
#include <iomanip>      // std::setprecision

using namespace std;

long double e(int x){

long double xx = 1, z, i = 1, yy = 0, y = 1;
	
	do{

	for(int lol = 0; lol < i; lol ++){

	yy = yy + 1;
	  y = y * yy;

}

	z = 1 / y;
	yy = 0;
	y = 1;
	xx = xx + z;
	i = i + 1;

	}while(i < x);

	return xx;
}

int main(){

int x, num;
double z;
	
	cout << "Calculuate_e" << endl;
	cout << "Number of decimal" << endl;
	cin >> x;
	num = x + 1;

 cout << "e = " << setprecision(num) << e(x) << '\n'; // Cuantos espacios de decimales imprimo

	return 0;
}
