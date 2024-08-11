## Input parsing ##

# Input format multiple lines int
```
n = int(input())
#Read the input
arr = []
i = n
while i > 0:
  a=int(input())
  arr.append(a)
  i = i - 1
```

## Enter multiple string data separated by space :


## taking three inputs at a time
```
x, Y, z = input("Enter three values: ").split() # default space separation
print(x + y + z)
```

## Enter two values (type int), separated by a space
```
a, b = map(int, input() split(" "))
print (a + b)
```

## Enter two values (type int) separated by commas
```
c, d = map(int, input().split(","))
print (c, d)
```

Sort array
Small to large: arr.sort()
Largest to smallest: arr.sort(reverse=True)

Len array
Returns the length of an array
```
X = len(array name)
print(x)
```

```
## n - row number in one line
n =  int(input())
M = []
for i in range(n):
  line = list(Map(int, input().split()))
  M.append(line)
```
```
## Output
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


