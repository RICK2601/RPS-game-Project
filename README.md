# RPS-game
Python Project - 

### Workflow Of Project ###
# 1 - Input from User ( Rock, paper, Scissor )
# 2 - Computer choice ( Computer choose randomly )
# 3 - Result Print

### Cases ###
# A - Rock
# Rock - Rock  = tie
# Rock - Paper = Paper win
# Rock - scissor = Rock win

# B - Paper
# Paper - Paper = tie
# Paper - Rock  = Paper win
# Paper - Scissor = Scissor win

# C - Scissor
# Scissor - Scissor = tie
# Scissor - Rock = Rock win
# Scissor - Paper = Scissor win
"-------------------------------------------------------------------------------"
import random

item_list = ["Rock", "Paper", "Scissors"]

user_choice = input("Enter your move (Rock, Paper, Scissors): ")
comp_choice = random.choice(item_list)

print(f"User choice = {user_choice}, Computer choice = {comp_choice}")


# Match / Tie
if user_choice == comp_choice:
    print("Both chose the same: Match / Tie")


# User chose Rock
elif user_choice == "Rock":

    if comp_choice == "Paper":
        print("Paper covers Rock = Computer wins")
    else:
        print("Rock smashes Scissors = You win")


# User chose Paper
elif user_choice == "Paper":

    if comp_choice == "Scissors":
        print("Scissors cut Paper = Computer wins")
    else:
        print("Paper covers Rock = You win")


# User chose Scissors
elif user_choice == "Scissors":

    if comp_choice == "Paper":
        print("Scissors cut Paper = You win")
    else:
        print("Rock smashes Scissors = Computer wins")


else:
    print("Invalid choice! Please enter Rock, Paper, or Scissors.")

