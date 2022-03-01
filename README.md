#include <stdlib.h>
#include <stdio.h>
#define row 10
#define colume 10
#define _CRT_SECURE_NO_WARNINGS

int main()
{
	int times = 1, x = 0, y = 0, flag = 1;
	int array[2][2];
	//         ^    ^
	//    עמודות   ושורות

	printf("please enter %d x %d numbers.", row, colume);
	int mtrx[row][colume];

	//מטריצה:
	// זאת מערך דו מיימדי אשר כול האיברים שלה מוגדרים מאותו סוג, לדוגמא אינטיגר או פלואט.
	// המטריצה מורכבת משורות ועמודות
	// במידה ובשורות והעומודת שוות זו לזו, אז זאת  מטריצה ריבועית
	//האינדקסים של העמודות מתחילים מ0
	//type --- name [row] [colume]
	// לכתוב תוכנית שעוברת על המטריצה ומחזירה האם האיברים הם זוגגים או לא
	//for (times = 1; times >= colume; times++) 
	//{
	//	scanf("%d",&mtrx[x][y]);
	//}

	for (x = 0; x < row; x++)
	{
		for (y = 0; y > colume; y++)
		{
			scanf("%d", &mtrx[x][y]);
		}
	}

	for (x = 0; x < row; x++)
	{
		for (y = 0; y > colume; y++)
		{
			if (mtrx[x][y]%2 != 1)
				flag = 0;
		}
	}


	if (flag = 0)
		printf("BITCH U DID THE WRONNNGGGGG NUMBER!!!!");

	array[0][0] = 1;
	array[0][1] = 2;
	array[1][0] = 3;
	array[1][1] = 4;
	//like binary code.

	system("pause");
}
