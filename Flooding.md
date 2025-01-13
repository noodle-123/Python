## Flooding matrix:
  1.Define matrix using 2 for loops for 2d array  
  2.Set range (scan matrix)  row by row
  3.Scan up (a[i-1][j]),left (a[i][j-1]),down(a[i+1][j]),right(a[i][j+1])  
  4.Make sure that all scanning areas are valid  check boundary:up(i>0) bottom(i<row) left(j>0) right(j<column)
  5.Save in another array (or else calculations will be affected)  
  
### Example code for scanning:
```
    for (int i = 0; i < n; ++i) {
        for (int j = 0; j < m; ++j) {
            int sum = 0;
            if (i > 0) sum += mat[i - 1][j];
            if (i < n - 1) sum += mat[i + 1][j];
            if (j > 0) sum += mat[i][j - 1];
            if (j < m - 1) sum += mat[i][j + 1];
            res[i][j] = sum;
```
