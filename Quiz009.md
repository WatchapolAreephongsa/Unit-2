```py

def missingNumber(n):
    for i in range(len(n)-1):
        if n[i]+ 1 != n[i+1]:
            result= n[i]+1
    return result

```
