# Game of Three java Client
# Notes :
- Java version 11 
- way of presentation is through console but it's decoupled from the logic
- built on top of Spring boot, used websocket for communication with other player
- Reacts upon events received from the subscribed topics
- players can play both automatically without inputs but only after
doing registration and start the game.

# Run steps:
- build with maven : mvnw install
- use the generated Jar in target folder and copy it with the number of clients
you want to try
- then run jars : java -jar client-X.X.X.jar
- you will be prompted to start new game from main menu
- register annonymously with nickname and play mode (auto / manual)
- wait other player to join (run another copy of client jar)
- then start play

# Game run sample:
```
======= Welcome to Game Of THREE !======= 
1) Start new game
2) Exit

Choose [1-2]: 
1
Please enter your nickname: 
yousef
Please choose your play mode (A/m): 
A: Auto
M: Manual
a
Please wait for your opponent to join ! 

(quit game? type exit)

Game is ready press any key to proceed

Your random starting number is : 71
please wait your turn

Now your turn !
Your opponent number reached 24 from his added number 72
Your auto pilot player choosed an addition move of 1
Your added number is 25
Not a valid move, Your added number is not divisible by 3 !
please wait your turn

Now your turn !
Your opponent number reached 8 from his added number 24
Your auto pilot player choosed an addition move of 1
Your added number is 9
Nice Move !, Your added number after division is 3
please wait your turn

Your opponent reached 1, You LOSE ! , Hard Luck yousef




Press ENTER key to continue
```
