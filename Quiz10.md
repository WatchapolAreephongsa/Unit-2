```py
def BigNeighbour(n):
    max = 0
    for i in range (1,len(n)):
        dif = n[i] - n[i-1]
        if dif > max:
            max = dif
    return max
```
