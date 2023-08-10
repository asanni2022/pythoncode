



```
max_trys = 3
trys = 0
pin = 4321

while trys < 3:
    entered_pin = int(input("Please enter your pin: "))
    trys += 1
    if len(str(entered_pin)) == 4:
        if str(entered_pin).isdigit():
            if entered_pin == pin:
                print("Hurrray! you have Zero bal left: 00.0 ")
                break
            else:
                print("you have entered an incorrect pin: "
                      + str(trys) + " attempt of 3 " )
        else:
            print("Invalid pin format. Please enter a numeric pin")
    else:
        print("Invalid pin length, Enter a 4 digit pin")
else:
    print("Sorry! max attempts card is retained contact your bank.")
```
