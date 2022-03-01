#include <stdlib.h>
#include <stdio.h>
#define row 3
#define colume 3
#define _CRT_SECURE_NO_WARNINGS

int main()
{
	int times = 1, x, y, flag = 1;
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
		for (y = 0; y < colume; y++)
		{
			scanf_s("%d", &mtrx[x][y]);
		}
	}

	for (x = 0; x < row; x++)
	{
		for (y = 0; y < colume; y++)
		{
			if (mtrx[x][y]%2 != 0)
				flag = 0;
		}
	}

	if (flag == 0)
		printf("BITCH U DID THE WRONNNGGGGG NUMBER!!!!");
	else
		printf("ur ok... ig");

	array[0][0] = 1;
	array[0][1] = 2;
	array[1][0] = 3;
	array[1][1] = 4;
	//like binary code.

	system("pause");
}
//מטלה: יש לכתוב תוכנית שקולטת מספרים במטריצה של מספרים שלמים מהמשתמש.
//התוכנית בסוף תדפיס את מספר האיברים הזוגיים במטריצה ואת המספרים האי זוגיים. (כמותם)
//היא תדפיס גם את כמות המספרים החיוביים והשלילים.
כלומר- חיובי, שלילי, זוגי, ואי זוגי.
