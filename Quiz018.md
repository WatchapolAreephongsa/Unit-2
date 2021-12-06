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
output = sum_array([1,2,3,4,6,2,7,1])
print(output)

```

# Output

<img width="953" alt="Quiz18" src="https://user-images.githubusercontent.com/82266864/144794002-47f90251-8263-4fc1-8ce8-d2e39ce7a8a3.png">

