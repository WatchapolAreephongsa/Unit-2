```py
def maxAbs(n):
    max = 0
    for i in range (len(n)):
        if abs(n[i])>max:
            max = abs(n[i])
    result = f"max absolute is {max}."
    return result
    
```
