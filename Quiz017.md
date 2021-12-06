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
output = validtri(1,1,2)
print(output)
```
# Output
<img width="759" alt="Quiz17" src="https://user-images.githubusercontent.com/82266864/144793917-1091c2c2-853b-4750-ac6e-d0ba03f98c4a.png">
