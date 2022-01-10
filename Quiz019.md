```py
#Function to give the inputted number to time and reverse it
def mirroredTime(time):
    #Limit the time to only possible hour which is 24
    if time<=24:
        #reverse for 1 digit number
        if time<10:
          #reverse for the number less than 6 which can be reverse else it will be more than 60 minutes which is not possible
            if time<6:
                result = f"0{time} : 0{time}, 0{time} : {time}0"
            elif time>=6:
                result = f"0{time} : 0{time}"
        #reverse for number more than 10
        if time> 10:
            #reverse for the last digit less than 6 else it will be more than or equal to 60
            if str(time)[0]!= str(time)[1] and int(str(time)[1])< 6:
                result = f"{time} : {time}, {time} : {str(time)[::-1]}"
            if str(time)[0]== str(time)[1] or int(str(time)[1])>=6:
                result = f"{time} : {time}"
    #For result that is not possible
    else:
        result = "None"
    return result
#Return result
output = mirroredTime(14)
print(output)
```

# Output
<img width="786" alt="Quiz198" src="https://user-images.githubusercontent.com/82266864/148713344-13cff149-e56e-45b4-8b54-5946f1751c1c.png">

# Flowchart

<img width="850" alt="Quiz19fc" src="https://user-images.githubusercontent.com/82266864/148716065-df88637b-4dd3-4430-b35b-36e8ef27aaee.png">
