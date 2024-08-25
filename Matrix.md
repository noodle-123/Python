#Scan Diagonally of a n*n matrix
```
n = int(input())
M = []
out = []
for i in range(n):
  line = list(map(int, input().split()))
  M.append(line)
row = []
for i in range(n):
  row.append(M[i][i])
out.append(row)
row = []
for i in range(n):
  row.append(M[n-1-i][i])
out.append(row)

for i in range(2):
  for j in range(n):
    print(out[i][j],end=" ")
  print()
```
