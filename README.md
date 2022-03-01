#include <stdlib.h>
#include <stdio.h>
#define row 4
#define colume 6

int main()
{
	int times = 1, x = 0, y = 0;
	int array[2][2];
	//         ^  ^
	//         עמודות ושורות

	int mtrx[row][colume];
	//מטריצה:
	// זאת מערך דו מיימדי אשר כול האיברים שלה מוגדרים מאותו סוג, לדוגמא אינטיגר או פלואט.
	// המטריצה מורכבת משורות ועמודות
	// במידה ובשורות והעומודת שוות זו לזו, אז זאת  מטריצה ריבועית
	//האינדקסים של העמודות מתחילים מ0
	//type --- name [row] [colume]

	for (times = 1; times >= colume; times++)
	{
		scanf("%d", mtrx[x][y]);

	}
	mtrx[0][0] = 1;
	mtrx[0][1] = 2;
	mtrx[1][0] = 3;
	mtrx[1][1] = 4;
	//like binary code.

	system("pause");
}
