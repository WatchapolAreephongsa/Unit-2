```py

def total (order, price):
    food = ["rice", "noodle", "bread", "fruit", "pizza", "hamburger", "sushi", "cake"]
    liquor =["beer", "wine", "sake", "champaign", "whiskey", "water", "soda", "juice"]
    electronic = ["ipad", "TV", "iphone", "speaker", "headphone", "play station"]
    total = 0
    for i in range(len(order)):
        #additional part for things that are not in the list.
        if order[i] not in food and order[i] not in liquor and order[i] not in electronic:
            category = input(f"{order[i]} not found, please put 1 if the item is food, 2 if the item is liquor and 3 if item is electronic.")
            if category == "1":
                food.append(order[i])
            if category == "2":
                liquor.append( order[i])
            if category == "3":
                electronic.append( order[i])
        if order[i] in food:
            price[i] *=1.1
        elif order[i] in liquor:
            price[i] *= 1.2
        elif order[i] in electronic:
            price[i]*=1.15
        total += price [i]
    Total = f"Total price is ¥{int(total)}."
    return Total


output = total(["Tesla car", "noodle", "champaign", "iphone", "vodka", "tea", "play station"] , [10000000 , 150, 4000, 80000, 3500, 140, 35000])
print(output)

``` 

# Output
<img width="1382" alt="Quiz13" src="https://user-images.githubusercontent.com/82266864/144793482-ab81eb49-25b2-4e53-a102-cb0c5881f630.png">


# Flowchart
![IMG_0222](https://user-images.githubusercontent.com/82266864/144940465-1a45b7e1-de4c-4f6c-92d8-dff7e9a584a4.JPG)
