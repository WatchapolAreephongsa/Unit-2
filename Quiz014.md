```py
def evenlySpread(a,b,c):
    if a<b<c or c<b<a:
        medium =b
        x1= a
        x2 =c
    if b<a<c or c>a>b:
        medium = a
        x1 = b
        x2 =c
    if b<c<a or a<c<b:
        medium = c
        x1 = a
        x2 = b
    if abs(medium-x1) == abs(medium-x2):
        result = "true"
    else:
        result = "false"
    return result

output = evenlySpread(2,4,6)
print(output)
```

# Sample outcome
true
