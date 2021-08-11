# Project1

# Project1

**Project 1 - Sports League Management Program - (100 points)**

Due date: September 27, 2021 at 11:59pm

**Objectives**

- Familiarize yourself with Files in Java
- Learn to use ArrayLists
- Practice with Strings

**Create a program to manage a League**

For this program, create a class League that includes the name of the league and a list of all the players in the league. You will also need to keep track of the number of players in your league. In addition to the getters/setters for the class, it will also contain the following methods:

```
1.  void addPlayer(Player newPlayer) - This method must be used to add new players to the league. Helpful note: This may be a good place to increment the counter for the number of players currently in the league.
2.  printLeague() - Print a list of all the players in your league. Make sure to use the Player class' toString() method for this.
3.  printAverageScore() - Calculate and print the average of all the players scores in the league.
```

**Player class**

The Player class will only contain the name of the player, the name of the team and the number of field goals made by the player. For this class, you need the constructor, getters/setters, and the toString() method.

**League - Driver class**

The driver class (LeagueDriver) will contain the main and must contain the following functionality:
- Read in the player information from an external text file. The name of the text file must be passed into the program through the command line arguments.
- Use a scanner to read in the file and to obtain the name, team name, and total field goals made for each player in the file.
- Invoke the printLeague() method to print a list of all the players in that league.
- Invoke the printAverageScore() method to display the average field goals made for the whole league.

**Reading the Player information from a file**

- Create a list of players (name, team, field goals) in a file on your computer. This file will be created as a separate text file in a text editor such as Sublime. For example, you may create a file (Players.txt) that contains the following:
```
Steph Curry, Golden State Warriors, 498, 
LeBron James, Cleveland Cavaliers, 484, 
Russell Westbrook, Oklahoma City Thunder, 459, 
James Harden, Houston Rockets, 449, 
```
- Read the file into your program. Refer to Section 5.5 from the textbook for how to use external files in your program.
- For the scanner that reads in from the file, the useDelimiter(", ") function will change the default delimiter from space to comma. 
- Since your final submission should have at least 6 players, this file should have at least six players too. Please do NOT make 6 separate Player objects in the League class. You have to use ArrayLists for this project. Since we will use ArrayLists, your program should be able to work with any number of players.
