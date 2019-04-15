# rock-paper-scissors
# First attempt at making a project, a simple Rock/Paper/Scissors using randit and elif statements!

from random import randit
player = raw_input("Rock (r), Paper (p), or Scissors (s)?")
print (player, 'vs')
chosen = randit(1,3)


if chosen == 1:
  computer = "r"
elif chosen == 2:
  computer = "p"
else:
  computer = "s"
  
if player == "s" and computer == "r":
  print "Rock crushes scissors, you lose!"
elif player == "s" and computer == "p":
  print "Scissors cut paper, you win!"
elif player == "p" and computer == "r":
  print "Paper covers rock, you win!"
elif player == "p" and computer == "s":
  print "Scissors cut paper, you lose!"
elif player == "r" and computer == "p":
  print "Paper covers rock, you lose!"
elif player == "r" and computer == "s":
  print "Rock crushes scissors, you win!"
else:
  print "Tie game, better luck next time!"
