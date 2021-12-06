```py

def missingNumber(n):
    for i in range(len(n)-1):
        if n[i]+ 1 != n[i+1]:
            result= n[i]+1
    return result
output = missingNumber([1,2,3,4,5,6,8,9])
print(output)
```

# Output
<img width="1165" alt="Quiz9" src="https://user-images.githubusercontent.com/82266864/144792776-f42c8ab9-11b3-468f-986a-ee54a31f35b5.png">
