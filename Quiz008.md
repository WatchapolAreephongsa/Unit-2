```py
def maxAbs(n):
    max = 0
    for i in range (len(n)):
        if abs(n[i])>max:
            max = abs(n[i])
    result = f"max absolute is {max}."
    return result
output = maxAbs([1,3,5,7,-2,4,-11001110111.1, -1111111])    
print(output)  
```

# Output
<img width="1400" alt="Quiz8" src="https://user-images.githubusercontent.com/82266864/144792719-15c757d4-b1e8-4dff-9546-b476735d7379.png">
