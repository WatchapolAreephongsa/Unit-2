```py

def swap(code):
    l = 0
    k = 1

    s_out = ""
    for i in range(len(code)//2):
        s_out += code[k] +code[l]
        k+= 2
        l+=2
    if len(code)%2 == 1:
        s_out += code[-1]
    return s_out

print(swap("1"))
```
