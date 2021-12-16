```py

def BlackBox(wrd):
    result = wrd[0]
    counter = 0
    for i in range (1,len(wrd)-1):
        if wrd[i+1]==" ":
            if counter != 0:
                result +=str(counter)
            result += wrd[i]
            counter = 0
        if wrd[i] == " ":
            result += wrd[i]
        if wrd[i-1] ==" " and wrd[i+1] != " ":
            result += wrd[i]
        elif wrd[i-1] != " " and wrd[i] != " " and wrd[i+1] != " ":
            counter+=1
    if counter != 0:
        result += str(counter)
    result += wrd[-1]
    return result

print(BlackBox("Hello World !"))
print(BlackBox("Internationalization"))
print(BlackBox("(codin) + (game) = (codingame)"))
print(BlackBox("localization"))
print(BlackBox("98 99 100 101 1062"))

```

# Outcome
<img width="831" alt="Q22" src="https://user-images.githubusercontent.com/82266864/146287694-de69e59d-f41e-4866-b3ca-abb0c0d9ecfc.png">
