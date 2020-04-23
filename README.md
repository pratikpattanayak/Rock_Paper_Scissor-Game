# Rock_Paper_Scissor-Game
This program helps two players to play rock ,Paper,Scissor game without letting anyone cheat



def Rock_Paper_Scissor(num1,num2,bit1,bit2):
    p1=int(num1[bit1])%3
    p2=int(num2[bit2])%3
    if(player_one[p1]==player_two[p2]):
        print("Draw")
    elif(player_one[p1]=="Rock" and player_two[p2]=="Scissor"):
            print("Player one wins")    #Rock crushes Scissor
    elif(player_one[p1]=="Rock" and player_two[p2]=="Paper"):
        print("Player two wins")        # Paper covers Rock 
    elif(player_one[p1]=="Paper" and player_two[p2]=="Scissor"):
        print("Player two wins")        #Scissor cuts Paper
    elif(player_one[p1]=="Paper" and player_two[p2]=="Rock"):
        print("Player one wins")
    elif(player_one[p1]=="Scissor" and player_two[p2]=="Rock"):
        print("Player two wins")
    elif(player_one[p1]=="Scissor" and player_two[p2]=="Paper"):
        print("Player one wins")
player_one={0:'Rock',1:'Paper',2:'Scissor'}
player_two={0:'Paper',1:'Rock',3:'Scissor'}
while(1):
    num1=input("Player one,Input your choice")
    num2=input("Player two,Input your choice")
    bit1=int(input("Player one,Enter secret bit position"))
    bit2=int(input("Player two,Enter your secret bit position"))
    Rock_Paper_Scissor(num1,num2,bit1,bit2 )
    ch=input("Do you want to continue? y/n")
    if(ch=='n'):
        break
    
