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

# Output
<img width="362" alt="Quiz14" src="https://user-images.githubusercontent.com/82266864/144793569-12eee52d-5d0c-4b1d-ae19-71428750a863.png">

# Flowchart
![IMG_0221](https://user-images.githubusercontent.com/82266864/144940408-de99ede2-801b-4a22-9db8-90992ed93ba0.JPG)
