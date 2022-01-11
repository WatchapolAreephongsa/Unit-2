```py
def Japanese_length(meters):
    m = float(meters[7:])
    meter = m
    Jap = ""
    shaku = 0.3030
    a = 0
    b = 0
    c = 0
    while m//shaku !=0:
       m-=shaku
       a += 1
    if a != 0:
        Jap += f"{str(a)} 尺"
    shaku/=10
    while m // shaku != 0:
        m = m - shaku
        b += 1
    if b != 0 and a!=0:
        Jap += f"and {str(b)}　寸"
    if b!= 0 and a == 0:
        Jap +=f"{str(b)} 寸"
    shaku /= 10
    while m // shaku != 0:
        m = m - shaku
        c += 1
    if c != 0 and (a!=0 or b !=0):
        Jap += f"and {str(c)}　分"
    if c!= 0 and (a == 0 or b == 0):
        Jap +=f"{str(b)} 寸"
    if a == 0 and b ==0 and c==0:
        Jap = "Unidentified"


    result = f"{meter} meters are apporximately {Jap} "
    return result
print(Japanese_length("meters=1.1223"))



```
