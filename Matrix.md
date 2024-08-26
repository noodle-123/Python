##Scan Diagonally of a n*n matrix##
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
# Output matrix
```
# print in rows
# M - matrix, n row numbers
for i in range(n):
  print(*M[i])

# ?
for i in range(3):
  for j in range(2):

    print(M[i][j],end=" ")
  print()

#Print without spaces or with designated seperator
```
Example- print w/ no space
print(M[i], sep = "")
```
# Matrix scan
#By row
```
n = row number, m = column number
for i in range(n):
    for j in range(m):
```
#By column
```
for j in range(m):
  for i in range(n):
```
#Access array element
Example: (taking 5th element)
```
1D array:
array[4]
# i is array index, n = array length
for  i  in range(0, n):

2D array:

```
#Boolean values
UPPERCASE

True
False
```
#Check matrix up, right, left, right
```
 if M[i][j-1] == 0 and M[i][j+1] == 0 and M[i-1][j] == 0 and M[i+1][j] == 0:
```

#Fill array with value, in this case, n*m array
```
M = [['o' for x in range(n)] for y in range(m)]
```
