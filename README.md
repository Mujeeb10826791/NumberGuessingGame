# NumberGuessingGame

import random

random_number = random.randint(0,50)
user_age = int(input("Please guess the number: "))

for i in range (5):
    if user_age == random_number:
        print("Congrates! You guess the correct number")
        break
    elif user_age < random_number:
        print("The number you enter is smaller")
        user_age = int(input("Please guess the number: "))
    else:
        print("The number you entered is greater")
        user_age = int(input("Please guess the number: "))
        
if user_age != random_number:
    print ("Sorry! you have used all your chances. the correct number is ", random_number)
