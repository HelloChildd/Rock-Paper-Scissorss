import random

comp_move = ['rock', 'scissors', 'paper']


user_wins = 0
comp_wins = 0
while user_wins != 5 and comp_wins != 5:
  q1 = input("\nEnter your move ,(rock,scissors,paper)")
  comp_choice = random.choice(comp_move)
  if (q1 == 'rock' and comp_choice == 'scissors') or (q1 == 'scissors' and comp_choice == 'paper') or (q1 == 'paper' and comp_choice == 'rock'):
    print ("Your Move :",q1)
    print ("Comp Move :",comp_choice)
    print ("YOU WIN")
    user_wins = user_wins + 1
    print ("Your score :",user_wins)
    print ("Comp score :", comp_wins)
    
  elif (comp_choice == 'rock' and q1 == 'scissors') or (comp_choice == 'scissors' and q1 == 'paper') or (comp_choice == 'paper' and q1 == 'rock'):
    print ("Your Move :",q1)
    print ("Comp Move :",comp_choice)
    print ("YOU LOSE")
    comp_wins = comp_wins + 1
    print ("Your score :",user_wins)
    print ("Comp score :", comp_wins)
    
  else:
    print ("Your Move :",q1)
    print ("Comp Move :",comp_choice)
    print ("YOU TIED")
    print ("Your score :",user_wins)
    print ("Comp score :", comp_wins)

