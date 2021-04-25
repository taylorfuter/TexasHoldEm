# TexasHoldEm
Texas Hold 'Em game developed for our final project of CSCI 201 at USC during Fall 2020. I collaborated with 5 other students to create the project in about 6 weeks. It features multithreading to allow multiple people to play at once, a database for users to log in, and a GUI that is friendly to the user. We also coded blackjack for guests to play. 

## INSTALLATION AND RUN 
Download .zip file from Piazza
Extract .zip file

### IMPORTING INTO ECLIPSE IDE:
Need to have Gradle Plugin installed
Install Buildship Gradle Integration 3.0 from Eclipse Marketplace 
Import
Gradle
Existing Gradle Project
Next
Next
Select the github folder “CS201L_TexasHoldemClient”
Next
Finish
You will have 4 Eclipse Projects now
Import
General
Existing Projects into Workspace
Select the folder “CS201L_pokerServerTester”

### TO RUN:
Start the server:
Go to CS201L_pokerServerTester > src/pokerServerTester/GameTestServer.java
Run
(Note: The server creates a mySQL database and fills it with three default users “username” (password: “password”), “Felipe” (password: “Felipe”), and “Jared” (password: “Jared”) and each new user is given $500 in betting money)


### Start the clients:
Open the Gradle Tasks Window (This should be automatically available in your Eclipse workspace when importing the Gradle project, otherwise go to Windows > Show View > Other > Gradle > Gradle Tasks)
Go through the file dropdown hierarchy  “CS201L_TexasHoldemClient-parent >  CS201L_TexasHoldemClient-desktop > application > run”. Double click to open a new client. (You may have to wait a few seconds for the workspace or Gradle plugin to load before it shows up).
Gradle will go through the building tasks, and when they have all been successfully completed, the client will start.
Run the client two more times for a total of 3 applications (This is needed to start the 3-player game)
Log in to a different account on each client
Once all three have authenticated their login credentials a game will begin.



## ONLINE GAMEPLAY:
The game follows the basic rules of Texas Holdem poker. Each player is dealt two cards hidden from other players  and a total of five cards are dealt onto the table over three rounds (the flop, the turn, and the river). Any combination of five cards in your hand or from the table can be used to gain the highest score to determine the winners
On your turn, the betting HUD will appear on the screen giving you the current betting information including the value of the pot, the total amount bet in the current round, the current betting value, the minimum value to raise by, the amount that you have bet this round, and the amount of funds you have left.
The HUD will give you your options which may be to bet (raise), call (match the current bet to stay in the game) or check (to keep the betting at the current amount), and to fold (to quit from the game). 
To bet, enter a valid number into the text box (must be a number greater than the minimum raise, but less than your remaining funds)
The rounds will continue through each player who hasn’t folded until all cards on the table are dealt and the betting has concluded
All active players’ cards will be revealed and the winner determined

## OFFLINE GAMEPLAY:
Select “Play Offline” from the main menu
A new game of blackjack will start against the computer dealer. (Feel free to click and drag the cards)
Click “Hit” to get another card and “Stay” to let the dealer play and end the game
Whoever has the highest value (Aces can be 1 or 11) without going over 21 wins
At the end of the game, a draggable window will pop up allowing you to keep playing or to go back to the main menu.
