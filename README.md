# Client-Server-Game
This is a client-server game built in java.
In this project, I used:
1 - Java networking.
2 - Java threading.
3 - Java databases.

It contain two packages:
Exercise1 package is about:
Write a client-server game, which provides “Guessing game” for two players against each other over TCP/IP network connection. The program has two main parts, the server and the client. The server handles the game. The server is available through a specified TCP port (3204) on specified machine by Guessing client. The server communicates the clients through socket connection and prints information to standard output. Only two players can connect to server at the same time and they can play with each other. If any additional player tries to connect to server, he will be refused. After the game, each player will be disconnected and they have to connect again if they want to play another game. The game starts when both players ready for game, therefore both players are connected. The game is very simple. Each player has a guessing number between 1 and 100, which must be found by the opponent. The players play the shared Guessing game alternately. The winner is whom the quickest to guess the guessing number chosen by the opponent. Players use the Guessing game client to play game through a consolebased interface as shown in Fig.1. First, the player can give the machine IP to access Guessing game server. Second, once accepted by the server, the player should enter his/her name and his/her guessing number. Third, each player, when his or her turn comes, must enter a positive number between 1 and 100. If one of the players would like to end prematurely the game, he/she should enter -1.  The server selects randomly the starting player and controls the turns of each player. Besides, the server informs who is the winner and tells each player the number of turn and whether he/she guessed too low, too high, or exactly right. 

Exercise2 package is about:
Modify the Exercise 1 so that the server will keeps players and the played games in a database. A player includes, an ID, and a name. A played game includes, an ID of the first player, an ID of the second player, the starting time of the game (for example 2020/5/13 17:20), the result of the game (1 if the first player won, 2 if the second player won, and 0 if the game has not been accomplished), the number of turns played. 
In this exercise, we assume that: 
 the player will enter his ID instead of his name. If the player is unrecognized he/she will be asked to enter his/her name in order to be added in the database.  
 for each player, and before starting the game the server will extract from the database and inform the client side by the following information:  
  o Player name 
  o Total number of games played by this player so far  
  o Best performance: Lowest number of turns played as a winner (if it exists)  
 
