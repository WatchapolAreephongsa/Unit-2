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

output = swap("10101-2ws")
print(output)
```
# Output
<img width="842" alt="Quiz16" src="https://user-images.githubusercontent.com/82266864/144793818-443aad37-55a5-4bbe-b2ef-f2784b732bff.png">
