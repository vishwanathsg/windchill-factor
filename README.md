# windchill-factor
This code tells the temperature that a living being experiences due to wind

#Factor:  Calculate temperature that a person feels because of the wind

Temp=float(input("Enter value for temperature in degree celsius: "))
#Took temperature input from the user

Vel=float(input("Enter velocity of wind speed (KMPH): "))
#Took velocity value from the user

if Vel<0:
    print("velocity of wind is invalid, try again")
    vel = float(input("Enter a positive velocity of wind speed (KMPH): "))

windchill=13.12+0.6215*Temp-11.37*Vel**0.16+0.3965*Temp*Vel**0.16
#Windchill factor formula

print("The temperature that a person will experience due to wind in the given condition is:", windchill )
