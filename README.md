# first-game-

print("Welcome to my first Game!")
name = input("Please enter your name: ")
age = int(input("Please enter your age: "))

health = 10

if age >= 18:
    print("You are allowed to play game")

    Wants_to_play = input("Do you want to play? ").lower()
    if Wants_to_play == "yes":
        print("You are starting out with",health,"health")
        print("Let's play the game")

        left_or_right= input("First choice is left or right (left/right)?")

        if left_or_right== "left":
            ans=input("Great, you followed the path and reached near a lake...Do you swim across or go around (across/around)?  ")
            if ans == "around":
                print("You went around the lake and reached the other side")
            
            elif ans == "across":
               print("You managed to get across, but were attacked by a fish and lost 5 health")
               health -= 5

            ans= input("You see a house and a river, where do you wanna go (house/river)? ")
            if ans=="house":
              print("You go near the house and the guy living in house attacked you and your health is reduced by 5 points")
              health-=5

              if health <=0:
                print("You now have 0 health and you lost the game")
              else:
                print("You have survied and won the game!")
              

            else:
              print("You go near the river and die")


        else:
            print("You fell down and lost")
        
    else:
      print("Ok byee....")

else:
  print("You are very small to play this game")

 


    
