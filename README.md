# Rock-Paper-Scissor-game
# Working

1. Imports:
import random: This line imports the random module, which provides functions for generating random numbers.

2. Introduction:
print("let's play Rock - Paper - Scissor"): This line prints a message to the console inviting the user to play Rock-Paper-Scissors.

3. User Input:
user_action=input("enter your choice(rock,paper,scissor): "): This line prompts the user to enter their choice (rock, paper, or scissor) and stores their input in the user_action variable.

4. Validating User Input:
possible_action=["rock","paper","scissor"]: This line defines a list called possible_action that contains the three valid choices (rock, paper, scissor).
if user_action not in possible_action:: This line checks if the user's input (user_action) is not present in the possible_action list.
print("please enter a valid response (rock,paper,scissor): "): If the input is invalid, this line prints an error message asking the user to enter a valid choice.

5. Computer's Choice (if user input is valid):
computer_action=random.choice(possible_action): This line uses the random.choice function to randomly select a choice for the computer from the possible_action list. The chosen action is stored in the computer_action variable.

6. Displaying Choices:
print(f'\nyou chose {user_action},computer chose {computer_action}'): This line uses an f-string to print a message that displays both the user's and the computer's choices.

7. Determining the Winner:
The code uses a series of if and elif statements to determine the winner based on the user's and computer's choices:
if user_action ==computer_action:: If both user and computer chose the same option, it's a tie. A message is printed accordingly.
elif user_action=="rock":: If the user chose rock:
if computer_action=="scissor":: If the computer chose scissor, rock wins. A winning message is printed.
else:: Otherwise (computer chose paper), paper covers rock, so the user loses. A losing message is printed.
Similar logic applies for elif user_action== "paper" and else: (user chose paper or scissor) with checks for computer's choices and corresponding win/lose messages.

Overall, this code provides a simple and interactive way to play Rock-Paper-Scissors against the computer in Python
