import random
'''
Stone, Paper, Scissors
'''
computer=random.choice(["s","p","sc"])
print('''

For Stone :- "s",
For Paper :- "p",
For Scissors :-"sc"
 
 
''')
userchoice=input("Enter your choice : ")
user_choice={"s":"Stone","p":"Paper","sc":"Scissors"}
print(f'''
You choose : {user_choice[userchoice]}
Computer choose : {user_choice[computer]}

''')

if(computer==userchoice):
    print("It's Draw !! ")
else:
    if(computer == "s" and userchoice == "sc"):
        print("You Lose🤦‍♂️!! ")
    elif(computer == "sc" and userchoice == "p"):
        print("You Lose🤦‍♂️!! ")
    elif(computer == "p" and userchoice == "s"):
        print("You Lose🤦‍♂️!! ")   
    elif(userchoice == "s" and computer == "sc"):
        print("You Win😎!! ")
    elif(userchoice == "sc" and computer == "p"):
        print("You Win😎!! ")
    elif(userchoice == "p" and computer == "s"):
        print("You Win😎!! ")
    else:
        print("Please enter a valid input 👀✔ ")  
   
        
