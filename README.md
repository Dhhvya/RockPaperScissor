Problem Statement
Python is a multipurpose language and one can do anything
with it. Python can also be used for game development. Let’s
create a simple command-line Rock-Paper-Scissor game
without using any external game libraries like PyGame. In this
game, the user gets the first chance to pick the option
between Rock, paper, and scissors. After the computer select
from the remaining two choices(randomly), the winner is
decided as per the rules. For getting random inputs from the
computer random module in python has been used in this
program which makes the game more interesting.


Methodology/Procedure
 The code starts by printing a message that states the
rules of the game.
 The first line in the code prints “Rock vs paper->paper
wins.”
 This is because if you have a rock, and you play against
someone who has a piece of paper, the rock will beat
the paper.
 The next line in the code prints “Rock vs scissor->Rock
wins.”
 This is because if you have a rock, and you play against
someone who has a scissors, the rock will beat the
scissors.
 The last line in the code prints “paper vs scissor->scissor
wins.”
 This is because if you have a piece of paper, and you
play against someone who has a scissors, then the piece
of paper will beat the scissors.
 The code will print the following output: Winning Rules
of the Rock paper scissor game as follows: Rock vs
paper->paper wins Rock vs scissor->Rock wins paper vs
scissor->scissor wins
 The code starts by asking the user for a choice.
 The code then checks to see if the input is 1, 2, or 3.
 If it is not one of those values, the code sets the
choice_name variable to ‘Rock’ if choice == 1, ‘paper’ if
choice == 2, and ‘scissor’ if choice == 3.
 The next part of the code asks the user for their
computer turn.
 The code uses a random number generator to choose
between 1, 2, and 3.
 This value is stored in comp_choice_name.
 Next, the code loops until comp_choice equals choice.
 In each loop iteration, comp_choice will be randomly
chosen from 1-3 and stored in comp_choice_name.
 Once comp_choice equals choice, this means that the
computer has chosen rock as its turn!
 Finally, it prints out both choices so that everyone can
see what happened (user choice is: Rock V/s paper;
Computer choice is: Rock V/s scissor).
 The code will ask the user for a choice between rock,
paper and scissors.
 Once the user enters their choice, the code will
randomly choose one of those options as the
computer’s turn.
 The code then prints out the chosen option and the
user’s choice.

Winning Rules as follows:
Rock vs paper-> paper wins
Rock vs scissor-> Rock wins
paper vs scissor-> scissor wins.
 In this game, randint() inbuilt function is used for
generating random integer values within the given
range.




Code (Python)
# import random module
import random
# Print multiline instruction
# performstring concatenation of string
print("Winning Rules of the Rock paper scissor
game as follows: \n"
+ "Rock vs paper->paper wins \n"
+ "Rock vs scissor->Rock wins \n"
+ "paper vs scissor->scissor wins \n")
while True:
print("Enter choice \n 1 for Rock, \n 2 for paper,
and \n 3 for scissor \n")
# take the input from user
choice = int(input("User turn: "))
# OR is the short-circuit operator
# if any one of the condition is true
# then it return True value
# looping until user enter invalid input
while choice > 3 or choice < 1:
choice = int(input("enter valid input: "))
# initialize value of choice_name variable
# corresponding to the choice value
if choice == 1:
choice_name = 'Rock'
elif choice == 2:
choice_name = 'paper'
else:
choice_name = 'scissor'
# print user choice
print("user choice is: " + choice_name)
print("\nNow its computer turn.......")
# Computer chooses randomly any number
# among 1 , 2 and 3. Using randint method
# of random module
comp_choice = random.randint(1, 3)
if comp_choice == 1:
comp_choice_name = 'Rock'
elif comp_choice == 2:
comp_choice_name = 'paper'
else:
comp_choice_name = 'scissor'
print("Computer choice is: " +
comp_choice_name)
print(choice_name + " V/s " +
comp_choice_name)
# we need to check of a draw
if choice == comp_choice:
print("Draw=> ", end="")
print("<== Its a tie ==>")
# condition for winning
if((choice == 1 and comp_choice == 2) or
(choice == 2 and comp_choice == 1)):
print("paper wins => ", end="")
print("<== User wins ==>")
elif((choice == 1 and comp_choice == 3) or
(choice == 3 and comp_choice
== 1)):
print("Rock wins =>", end="")
print("<== User wins ==>")
elif((choice == 2 and comp_choice == 3) or
(choice == 3 and comp_choice
== 2)):
print("scissor wins =>", end="")
print("<== User wins ==>")
else:
print("<== Computer wins ==>")
break
# after coming out of the while loop
# we print thanks for playing
print("\nThanks for playing")
Result
OUTPUT
Winning Rules of the Rock paper scissor game as
follows:
Rock vs paper->paper wins
Rock vs scissor->Rock wins
paper vs scissor->scissor wins
Enter choice
1 for Rock,
2 for paper, and
3 for scissor
User turn: 3
user choice is: scissor
Now its computer turn.......
Computer choice is: paper
scissor V/s paper
scissor wins =><== User wins ==>
Thanks for playing
Conclusion
Python in current times is used for developing websites and
software, task automation, data analysis, and data
visualization. Since it's relatively easy to learn, Python has
been adopted by many non-programmers such as
accountants and scientists, for a variety of everyday tasks,
like organizing finances. Therefore, with the help of a python
program we have created a Rock-Paper-Scissors game
