# Kaun-banega-crorepati
questions = [
  [
    "which is these is not a web browser", "firefox", "chrome", "facebook",
    "Opera", "None", 3
  ],
  [
    "Who is the No 1 Instagram followers in the world?", "Cristiano Ronaldo", "Leo Mess", "Kylie Jenner",
    "Selena Gomez", "None", 1
  ],
  [
    "Who is the NO 1 follower in Facebook?", "Cristiano Ronaldo", "Shakria", "Will Smith",
    "Vin Diese", "None", 1
  ],
  [
    "who is the richest person in the world?", "jeff Bezos", "Elon musk", "Warrent Buffet",
    "lary ellison", "None", 2
  ],
  [
    "Richest Actor in the world?", "shah Rukh khan", "Tyler perry", "jerry seinfeld",
    "Dwayne johnson", "None", 3
  ],
  [
    "Which language was used to create fb?", "Python", "French", "JavaScript",
    "Php", "None", 4
  ]
  
]

levels = [1000,10000, 100000, 5000000,10000000,70000000]
money = 0
for i in range(0, len(questions)):
  
  question = questions[i]
  print(questions[i])
  print(f"\nAbove Question for Rs. {levels[i]}")
  print(f"1. {question[1]}          2. {question[2]} ")
  print(f"3. {question[3]}          4. {question[4]} ")
  reply = int(input("Enter your answer (1-4) or  0 to quit:\n" ))
  if (reply == 0):
    money = levels[i-1]
    break
  if(reply == question[-1]):
    print(f"Correct answer, you have won Rs. {levels[i]} \n")
    if(i == 1):
      money = 10000
    elif(i == 3):
      money = 5000000
    elif(i == 5):
      money = 70000000
  else:
    print("Wrong answer!")
    break 

print(f"Your take home money is {money}")






