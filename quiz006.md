```py
def letters(word):
    hello = []
    for i in range (len(word)):
        hello.append(f"{i} -> {word[i]}")

    return hello
print(letters('hello'))
```
