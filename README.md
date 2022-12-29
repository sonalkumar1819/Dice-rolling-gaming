# Dice-rolling-gaming
import random
sum,win =0, 0 #initialize()
while True:
 num = random.randint(1, 6) #picking randomly integer in the given interval
 x = input("Enter 'no' to exit or any other key to play: ")
 if x =="no":
  break
 sum=sum+1
 n = int(input("Guess number b/w 1 to 6: "))
 if n > 6:
  print("Entered invalid number hence 'Exit'")
  break
 if num == 1:
  print("[-----]")
  print("[     ]")
  print("[  o  ]")
  print("[     ]")
  print("[-----]")
 elif num == 2:
  print("[-----]")
  print("[o    ]")
  print("[     ]")
  print("[    o]")
  print("[-----]")
 elif num == 3:
  print("[-----]")
  print("[o    ]")
  print("[  o  ]")
  print("[    o]")
  print("[-----]")
 elif num == 4:
  print("[-----]")
  print("[o   o]")
  print("[     ]")
  print("[o   o]")
  print("[-----]")
 elif num == 5:
  print("[-----]")
  print("[o   o]")
  print("[  o  ]")
  print("[o   o]")
  print("[-----]")
 elif num == 6:
  print("[-----]")
  print("[o o o]")
  print("[     ]")
  print("[o o o]")
  print("[-----]")
 if num == n:
  win=win+1 #game win ;
  print("winner ...")
  print("No. of times played:", sum)
  print("No. of times won:", win)
 else:
  print("plse try again........Give me your best")
print("Game Summary:--->")
print("No. of times played:", sum)
print("No. of times won:",win)
