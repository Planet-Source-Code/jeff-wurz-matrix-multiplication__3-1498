<div align="center">

## Matrix Multiplication


</div>

### Description

It takes a user inputed matrix and multiplys it by another user inputed matrix producing a matrix...
 
### More Info
 
can get some warnings in compilers... its just cause of the way i had to program it... the reinitializing of the matrices


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jeff Wurz](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jeff-wurz.md)
**Level**          |Intermediate
**User Rating**    |4.2 (25 globes from 6 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jeff-wurz-matrix-multiplication__3-1498/archive/master.zip)

### API Declarations

```
#include <iostream.h>
```


### Source Code

```
#include <iostream.h>
int main()
{
int cols = 3, rows= 2, colss= 2, rowss= 3;
int var = 0;
cout << "Enter in the number or rows for the first matrix: ";
cin >> cols;
cout << "Enter in the number or columns for the first matrix: ";
cin >> rows;
	int mat[2][2];
	mat[rows-1][cols-1];
	for(int row = 0; row <= rows-1; row++)
		{
		for(int col = 0; col <= cols-1; col++)
			{
			cout << "Enter the value for the element of row " << row + 1 << " and column " << col + 1 << " of the first matrix: ";
			cin >> var;
			mat[row][col] = var;
			cout << '\n';
			}
		}
cout << "Enter in the number or rows for the second matrix: ";
cin >> colss;
cout << "Enter in the number or columns for the second matrix: ";
cin >> rowss;
	int matr[2][2];
	matr[rowss-1][colss-1];
	for(row = 0; row <= rowss-1; row++)
		{
		for(int col = 0; col <= colss-1; col++)
			{
			cout << "Enter the value for the element of row " << row + 1<< " and column " << col + 1<< " of the second matrix: ";
			cin >> var;
			matr[row][col] = var;
			cout << '\n';
			}
		}
int matri[2][2];
matri[rows][rowss];
matri[1][0]	= 0;
int vect[2];
for(int xvar = 0; xvar <= rows; xvar++)
	{
	for(int yvar = 0; yvar <= cols; yvar++)
		{
		for(int xvari = 0; xvari <= rowss; xvari++)
			{
		for(int yvari = 0; yvari <= colss; yvari++)
				{
			vect[yvar] = mat[xvar][yvar] * matr[yvari][xvari];
				}
			}
		}
	for(int vecto = 0; vecto <= rows; vecto++)
		{
			for(int xvect = 0; xvect <= rows; xvect++)
			{
			for(int yvect = 0; yvect <= rows; yvect++)
				{
				matri[xvect][yvect] = vect[vecto];
				}
			}
		}
	}
	cout << "\n";
	for (rows = 0; rows < 2; rows++)
	{
		for (cols = 0; cols < 2; cols++)
		{
			cout << matri[rows][cols] << "   ";
		}
		cout << endl;
	}
return 0;
}
```

