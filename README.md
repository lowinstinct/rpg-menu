# rpg-menu
# Oluwatimileyin Soyege
# Computer Science 30
# Mrs Cotcher
# 5 October 2021







input("welcome to the game, please press start")


def game_instructions():
  
   
   #print a main menu and the commands
   
   print("Avenging Death Adventure Game")
   
   print("You have meet the Killer who killed your family, choose the best option to respond to")
   
   print('you have four options: shoot, stay, call, or exit, which one shall you pick?')
   
   
   print("Add to Inventory: get 'item name'")

game_instructions()


options = {
          
          
          
          #first option, you shoot the killer bringing justice
          
          
          
          "1": {
                'choice':'shoot',
                'decision':'killer has been shot right in the heart',
                'result':'family death avenged, game over'},   
          
          
          
          
          #in the second option you decide to stay with the killer
          
          
          "2": {
                'choice':'stay',
                'decision':'shoot six times',
                'result':'game over you lose'},
          
# Adding new dictionaries in the option dictionary

# in the third option we call the police
          
          
          "3": {
                'choice':'call the police',
                'decision': 'beat up the killer',
                'result':"killer has been arrested, game over"},

# in the fourth option you exit the program, which means you wont get to play the game
          
          
          
          "4": {
                'choice':'exit',
                'decision':'no decision', 
                'result':"you have exited the program"}
           }



for numbered_choice in options:
    print(f"{numbered_choice}. {options[numbered_choice]['choice']}")
    print(f"{numbered_choice}. {options[numbered_choice]['decision']}")
    print(f"{numbered_choice}. {options[numbered_choice]['result']}")





for numbered_choice in options:
    for action in options[numbered_choice]:
        print(f"{numbered_choice}.{options[numbered_choice][action]}")



input("please continue")




characters = {'You':{
                'name' : "Chris",
                'race' : "Black",
                'lvl': 1,
                'xp': 0,
                'lvlNext' : 25,       
                'stats' : {
                        'str': 1,
                        'dex' : 1,
                        'int' : 1,
                        'atk' : 12,
                        'hp' : 20,
                        'maxHp' : 20},      
                'inv' : {
                        'Black': 32,
                        '200' : ' 6 ft' }
                     },
              "Killer":{
                'name' : "Ryan",
                'ace' : "White",
                'lvl': 2,
                'xp': 80,
                'stats' : {
                        'atk' : 6,
                        'hp' : 15,
                        'maxHp': 15},
                 'inv': {
                        'White': 31,
                        '163': '5 ft',}
                        }
               }



for k, v, in characters['You']['inv'].items():
    print("\n------You-----")
    print("Race:", k )
    print("age:", v)
for w, h, in characters['You']['inv'].items():
    print("Weight:", w )
    print("Height:", h)
    print("-----Chris-----")


for k, v in characters ['Killer']['inv'].items():
    print("\n-----Killer-----")
    print("Race:", k )
    print("Age:", v)
for w, h, in characters['Killer']['inv'].items():
     print("Weight:", w )
     print("Height:", h)
     print("-----Adam-----")





input("please continue")



location = [ "Eagle Street", "Brooklyn", "New York", "USA" ]

print(location)     # prints all elements


print(location[0])  # print first element


print(location[1]) # print second element


print(location[2]) # print third element 


print(location[3]) # print fourth element
