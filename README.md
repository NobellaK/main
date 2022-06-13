# main
# Import python modules
from random import randint

user_action = input("Enter a choice (R, P, S): ")
possible_actions = ["Rock", "Paper", "Scissors"]
computer_action = possible_actions[randint(0,2)]

print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")

player = False 
while player == False:
    player = user_action 
    if player == computer_action:
        print("Tie!")
    elif player == "Rock":
        if computer_action == "Paper":
            print("Try Again")
        else:
            print("You win!")
    elif player == "Paper":
        if computer_action == "Scissors":
            print("Try Again")
        else: 
            print("You win!")
    elif player == "Scissors": 
        if computer_action == "Rock":
            print("Try Again")
        else: 
            print("You win!")
    
    else:
        print("Thats an invalid play. Check your input!")
    
    # Player was set to False so the loop continues





