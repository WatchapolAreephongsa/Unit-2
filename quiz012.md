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

# Sample Outcome

4.5
