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
