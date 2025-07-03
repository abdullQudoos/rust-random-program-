def maximum(v1,v2,v3):
    max_value = v1
    if v2 > max_value:
        v2 = max_value
    if v3 > max_value:
        v3 = max_value
    return max_value
print(maximum(2,3,5))

 min(15, 9, 27, 14)
#___________________________________________________________ 
import random
frequency1 = frequency2=frequency3=frequency3=frequency5=frequency6 = 0

for roll in range(600,000):
  face = random.randrange(1, 10)
   
  if face == 1:
      frequency1 +=1
  elif face == 2:
      frequency2 +=1
  elif face == 3:
      frequency3 +=1
  elif face == 4:
      frquency4 +=1
  elif face == 5:
      frequency5 +=1
  elif face == 6:
       
      frequency6 +=1
print(f"face{"frequency1":>13}")
print(f"{1:>4}{frequency1:>13}")
print(f"({2:>4}{frequency2:>13}")
# print(f"{3:>4}{frequency3:>13}")
# print(f"{4:>4}{frequency4:> 13}")
# print(f"{5:>4}{frequency5:>13}")
# print(f"{6:>4}{frequency6:>13}")

import random 
frequency1= frequency2=frequency3=frequency4=frequency5=frequency6 = 0

for roll in range(600,00):
    face  = random.randrange(1,7)
    
    if face == 1:
        frequency1 += 1
    elif face == 2:
        frequency +=1
    elif face == 3:
        frequency3 +=1
    elif face ==4 :
        frequency4 +=1
    elif face == 5:
        frequency5 +=1
    elif face == 6:
        frequency6 +=1
print(f"face{"frequency":>13}")
print(f"{1:>4}{frequency1:>13}")
print(f"{2:>4}{frequency2:>13}")
print(f"{3:>4}{frequency3:>13}")
print(f"{4:>4}{frequency4:>13}")
print(f"{5:>4}{frequency5:>13}")
#_--------------------------------------------------
import random

random.seed(123)  # تنظیم مقدار seed

print(random.random())        # همیشه همان عدد را چاپ می‌کند
print(random.randint(1, 100))


import random
for i in range(20):
    
    if random.randrange(2)== 0:
        print("H", end= " ")
    else:
        print("T", end = ' ')

import random
def roll_dice():
    die1 = random.randrange(1, 7)
    die2 = random.randrange(1, 7)
    return (die1, die2)
def display_dice(dice):
    die1, die2 = dice
    print(f'Player rolled {die1} + {die2} = {sum(dice)}')
die_values = roll_dice()
display_dice(die_values) 
sum_of_dice = sum(die_values)
if sum_of_dice in (7, 11):
    game_status = 'WON'
elif sum_of_dice in (2, 3, 12):
    game_status = 'LOST'
else:  # remember point
    game_status = 'CONTINUE'
    my_point = sum_of_dice
    print('Point is', my_point)
 # continue rolling until player wins or loses
while game_status == 'CONTINUE':
    
     
     
     
    die_values = roll_dice()
    display_dice(die_values)
    sum_of_dice = sum(die_values)
    if sum_of_dice == my_point:
        game_status = 'WON'
    elif sum_of_dice == 7:
        game_status = 'LOST'
 # display "wins" or "loses" message
    if game_status == 'WON':
        print('Player wins')
    else:
        print('Player loses')        
        
        
    
