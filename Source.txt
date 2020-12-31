#include<iostream>
#include<conio.h>


using namespace std;
int main() {
	int data[4][10] = { {401,21000,42000},{402,0,59000},{403,12000,19000,21000},
	{404,56000} };
	
	
	for (int row = 0; row < 4; row++) {
		int sum=0;
        for (int col = 1; col < 9; col++) {
			sum = sum + data[row][col];
			
		
		}
data[row][9] = sum;
	}
		

	for (int j = 0; j < 4; j++) {
		cout << "2015-CS-" << data[j][0] << "   Paid fee Rs ." << data[j][9] << "/-" << endl;
	}

	_getch();

}
