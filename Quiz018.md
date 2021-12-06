```py
def sum_array(numbers:list)->int:
    sum = 0
    skip = 0
    for i in range(len(numbers)):
        if numbers[i] == 6:
            skip = 1
        if skip == 0:
            sum += numbers[i]
        if numbers[i] == 7:
            skip = 0
    return sum

print(sum_array([1,2,3,4,6,2,7,1]))

```
