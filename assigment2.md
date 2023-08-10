### Assignment2
## Bank ATM Operations.

Objective: Create a simulation of an ATM where the user needs to enter a PIN to access their account.

Inputs:

1. PIN - A numeric (or alphanumeric) code that the user needs to input. The correct PIN is set in the program.

Outputs:

1. Access status - Whether the user inputted the correct PIN or not.

2. Attempts left - If the PIN is incorrect, how many attempts they have left.

Requirements:

1. The user gets three attempts to enter the correct PIN.
2. If the user fails three times, inform them their card is retained and they need to contact their bank.
3. If the PIN is correct, grant them access.
4. If the user inputs a non-numeric PIN (unless you allow alphanumeric PINs), prompt them to input a valid PIN.
5. For security reasons, don't display the PIN they entered. Instead, use placeholders like **.

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
