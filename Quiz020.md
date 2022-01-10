
```py
def ScientifiNot(number:int) -> str:
    #Change that number to the scientific notation form.
    num = str(number)
    a = 1
    #for number less than 1000
    if len(num)>=3:
        result = f"{num[0]}.{num[1]}{num[2]} * 1e{len(num)-1}"
    #For number more than 1000
    else:
       while len(num)!=3:
            num += "0"
            #a or the exponent of 10 will be 1 less than the number of digit
            a +=1
       result = f"{num[0]}.{num[1]}{num[2]} * 1e{len(num) - a}"
    return result

output = ScientifiNot(12000)
print(output)
```

# Sample Output

<img width="905" alt="QUiz" src="https://user-images.githubusercontent.com/82266864/148713952-3f28d66d-f27a-47a9-8870-4db652d0b02b.png">

# Flowchart

<img width="670" alt="Quiz20" src="https://user-images.githubusercontent.com/82266864/148732453-8fc6bf2f-3f9a-4aea-b52c-2bbfb4276e0a.png">
