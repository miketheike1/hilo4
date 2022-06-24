# Python3 program to demonstrate the use of
# choice() method
 
# import random
import random
randomint = 1
score = 1
over = True 
randomnum = 1 
# 
#  a random value from the list
def randomnum1():

    list1 = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10 , 11, 12, 13]
    randomint = random.choice(list1) 

# prints a random item from the string
    return randomint 
def randomnum2():

    list1 = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10 , 11, 12, 13]
    randomint = random.choice(list1) 

# prints a random item from the string
    return randomint 

def main():
    score = 0
    over = True
    randomint1 = randomnum1()
    randomint2 = randomnum2()
    print("Welcome to HiLo!")

    while (over == True): 
    
        print("The card is: ",randomint1)
        choice = str(input("Higher or Lower [H/L]:"))

        if choice == "H".lower() and randomint1 >=  randomint2:
            score = score + 100
        else:
            score = score - 75 

        if choice == "L".lower() and randomint1 <=  randomint2:
            score = score + 100
        else: 
            score = score - 75 
        
        print("Your score is: ",score)
        play = str(input("Play again: [Y/N]"))
        if play == "Y".lower():
            over = True 

        elif play == "L".lower():
            over = False 
            

    

if __name__ == "__main__":
    main()
