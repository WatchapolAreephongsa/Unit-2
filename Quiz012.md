```py
def wordlength(word):
    avg= 0
    length = 0
    for i in range(len(word)):
        length += len(word[i])
    avg = length/len(word)
    return avg

output = wordlength(["home", "car", "travel", "beach"])
print(output)
```

# Output
<img width="896" alt="Quiz12" src="https://user-images.githubusercontent.com/82266864/144793403-73f450aa-26f4-419e-86fa-5d0552270aae.png">

