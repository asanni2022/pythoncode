# pythoncode
### Assignment1
1. Temperature Converter
Objective: Create a program that can convert temperatures between Fahrenheit, Celsius, and Kelvin.

Inputs:
Initial temperature scale - Ask the user to provide the scale of the temperature they're starting with (Fahrenheit, Celsius, or Kelvin).

Temperature value - The actual numeric temperature in the scale provided above.

Target temperature scale - Ask the user the scale they wish to convert the above temperature to (Fahrenheit, Celsius, or Kelvin).

Outputs:

The converted temperature value in the target scale.

Requirements:

1. The converter should be accurate.
2. If the user inputs an invalid scale (not one of the three), the program should prompt them to input a valid scale.
3. Consider edge cases (e.g., absolute zero).
```
initial_scale = input("Enter Temp Initial scale: ")
temperature = int(input("Enter Temp Value:  "))
target_scale = input("Enter Temp target scale: ")

if initial_scale == 'Fahrenheit':
    if target_scale == 'Celsius':
        converted_temp = (temperature - 32) * 5 / 9
        print("Temp Fahrenheit in Celsius:  " + str(converted_temp))
    elif target_scale == 'Kelvin':
       converted_temp = (temperature - 32) * 5 / 9 + 273.15
       print("Temp Fahrenheit in Kelvin:  " + str(converted_temp))
    else:
        print("Invalid target scale")
elif initial_scale == 'Celsius':
    if target_scale == 'Fahrenheit':
        converted_temp = (temperature * 9 / 5) + 32
        print("Temp Celsius in Fahrenheit:  " + str(converted_temp))
    elif target_scale == 'Kelvin':
        converted_temp = temperature + 273.15
        print("Temp Celsius in Kelvin:  " + str(converted_temp))
    else:
        print("Invalid target scale")
elif initial_scale == 'Kelvin':
    if target_scale == 'Fahrenheit':
        converted_temp = (temperature - 273.15) * 9 / 5 + 32
        print("Temp Kelvin in Fahrenheit:  " + str(converted_temp))
    elif target_scale == 'Celsius':
        converted_temp = temperature - 273.15
        print("Temp Kelvin in Calcius:  " + str(converted_temp))
    else:
        print("Invalid target scale")
else:
    print("Invalid target scale")
```

### Assignment2
Bank ATM Operations
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
