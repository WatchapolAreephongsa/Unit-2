```py
def reverse_mode(num):
    A = (4*int(num[0])) + 2 * (int(num[1])) + (int(num[2]))
    B = (4*int(num[4])) + 2 * (int(num[5])) + (int(num[6]))
    C = (4*int(num[8])) + 2 * (int(num[9])) + (int(num[10]))
    result = str(A)+ str(B)+str(C)
    return result

print(reverse_mode("100!000!000"))
```
