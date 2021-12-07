```py
def BigNeighbour(n):
    max = 0
    for i in range (1,len(n)):
        dif = n[i] - n[i-1]
        if dif > max:
            max = dif
    return max
output = BigNeighbour([1,2,103,5,6,7])
print(output)
```
# Output
<img width="1180" alt="Quiz10" src="https://user-images.githubusercontent.com/82266864/144793298-a9ae9a18-dc1a-4c39-b755-52836e3aade3.png">

# Flowchart
![PNG image 2](https://user-images.githubusercontent.com/82266864/144941767-214e3385-7652-46d7-845e-f67d2542cdee.png)

