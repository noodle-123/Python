
## DFS

```
def dfs(nums, visited, subset, result):
  if len(subset) == len(nums):
    result.append(subset)
    return 

  for i in range(0, len(nums)):    
    if visited[i]:
      continue
    if subset:
        if nums[i] != subset[-1]+1 and nums[i] != subset[-1]-1:   
           subset.append(nums[i])
           visited[i]=True
           dfs(nums, visited, subset, result)
           subset.pop()
           visited[i]=False
        else:
           continue
    else:
       subset.append(nums[i])
       visited[i]=True
       dfs(nums, visited, subset, result)
       subset.pop()
       visited[i]=False
  ```
