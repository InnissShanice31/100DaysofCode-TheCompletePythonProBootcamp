print(r'''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\ ` . "-._ /_______________|_______
|                   | |o ;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to New York City.")
print("Your mission is to find the treasure.")
choice1 = input('You\'re stuck in a New York alley, which direction do you want to go in? '
                'Type "left" or "right".\n').lower()

if choice1 == "left":
    choice2 = input('You\'ve come to a street. '
                    'There is rabid dog in the middle of the street. '
                    'Type "wait" to wait on animal control. '
                    'Type "run" to run away.\n').lower()
    if choice2 == "wait":
        choice3 = input("Animal control tells you that they are on the way but will take some time. "
                        "They tell you to wait 30 minutes. "
                        "You could also run or fight the dog. "
                        "Which option do you choose do you choose?\n").lower()
        if choice3 == "wait 30 minutes":
            print("You are bitten and die. Game Over")
        elif choice3 == "run":
            print("You made it away safely. You Win!")
        elif choice3 == "fight the dog":
            print("The dog is too strong, you loose the fight, get bitten and die. Game Over.")
        else:
            print("You chose an option that doesn't exist. Game Over.")
    else:
        print("You got bitten anyway. Game Over.")

else:
    print("You got robbed and killed by New York crack heads. Game over")
