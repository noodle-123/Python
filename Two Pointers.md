# Python
Two Pointers
```
 i = 0 #Left pointer
 j = len(s) - 1 #Right pointer
 while i < j: #While loop: Switch until they meet
     temp = s[i] 
     s[i]=s[j]
     s[j]=temp
     i+=1 #Switch index
     j=j-1
        
```
