```py
def SameFirstLast(n):
    if len(n)>1 and n[0] == n[-1]:
        result = "TRUE"
    else:
        result = "FALSE"
    return result
output = SameFirstLast([1,1])
print(output)
```
# Sample Outcome
TRUE
