## Matrix ##
```
# Input
# n - row number in one line
n =  int(input())
M = []
for i in range(n):
  line = list(Map(int, input().split()))
  M.append(line)
```
```
# Output
# print in rows
# M - matrix, n row numbers
for i in range(n):
  print(*M[i])

# ?
for i in range(3):
  for j in range(2):

    print(M[i][j],end=" ")
  print()
```


