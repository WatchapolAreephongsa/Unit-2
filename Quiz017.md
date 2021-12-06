```py
def validtri(a,b,c):
    if b>a and b>c:
        if a+c > b:
            result = "true"
        else:
            result = "false"
    if a>b and a>c:
        if b+c > a:
            result = "true"
        else:
            result = "false"
    if c>a and c>b:
        if a+b > c:
            result = "true"
        else:
            result = "false"
    return result
print(validtri(1,1,2))
```
