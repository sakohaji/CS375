# CS375
Software engineering
from random import random


def HoopsDrill():

    shots = [] #Random list that has data of the shots
    miss_shot = 0
    make_shot = 1
    #wins =   #this will count the wins/losses so later we can calculate averages and probability
    #losses = 

    for i in range(100):
        shots.append( int(random() + 0.5) ) #Random generator appends into list
  
        if ( len(shots)>2 and shots[i]==1 and shots[i-1]==1 and shots[i-2]==1 ): #Compares the current i with the two previous ones
            print ("you win")

        elif (len(shots)>2 and shots[i]==0 and shots[i-1]==0 and shots[i-2]==0):
            print ("you lose")
        else:
            print ("keep going")

        print (shots)
        
HoopsDrill() #Calls the function
