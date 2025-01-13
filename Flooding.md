#Flooding matrix:
  1.Define matrix using 2 for loops for 2d array
  2.Set range (scan matrix)
  3.Scan up,left,down,right
  4.Make sure that all scanning areas are valid
  5.Save in another array
  6.Output
#Example code for scanning:
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
