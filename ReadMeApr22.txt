This program is designed to simulate a card game Adventure Games: Discover the story. The objective of the game 
is to reach the end of the story by performing a series of actions that mostly involve combining item with 
another item and sometimes another location. The game can support 1-4 players. If there is just one player, he 
or she will have to play with two characters. The way the game consists of a variety of different cards such as
rooms, items, characters, health, objectives, and events. All the cards are labeled on one side to avoid spoiling 
the story of the game when searching for a specific card. 


	How the game normally works
The beginning of the game starts with room card A being set down and having all character pieces, that are being
played, placed there. Depending on the number of people playing, all characters have a specific amount of health.
The more people that play, the less health each person starts with. Then you have the entry book that contains all 
the information on rooms, introductions to areas, events, and item combinations with areas. Once the pieces are set
up, players will read the first entry that assigns them a mission card, that explains to them their objective, and 
read an entry on the room to show what they can interact with. 

Each player can do one of the following actions
-Explore a location number. This involves the player reading the entry book for the specific location number.
(example 801). This leads to a better understanding of the story and sometimes recieve items.

-Combine item with another item. Combining items, adventure cards, involves taking the ids of the card and combining
them together, lowest number first, and reading the entry of the number in the book.

-Combine item with a location. Combining these two works the same way with combining two adventure cards together. 
Room card ids have three digits, so item card ids are always combined first.

Players can move to a location freely on their turn and then perform an action if desired.

This adventure game consists of three chapters (objectives) and a session ends after one chapter. After the chapters 
are complete, the score is then calculated. Points are awarded usually by finding items or by performing certain 
actions.


	How our program simulates the game
The biggest portion of the game comes from the entry book. It holds all information regarding outcomes of the 
player's actions. So, we designed several functions to hold the entries that are in the entry book. These 
functions are made up of a switch statement handling each case like an entry. However, because a variety of 
different things that can happen with these entries, all information about the player's inventory and health 
need to be sent to the function by reference. For each of these entries, a message box is displayed to inform the
player of the outcome. The following functions follow the same format described from above.
-Entry evaluation function
-Item combination function
-Item Location function

The main driver starts up the GUI applications as well as connect all the external classes involving entries.

	GUI walkthrough
Our program starts with the first window showing the front cover of the game and a single button. Once this 
button is pressed, the character selection window starts and the initial window becomes hidden. In this window, 
there are a number of characters to choose from. Initially, the game is designed for just one person, so the user 
gets to choose an initial character to start with and the remaining buttons are replaced with check boxes. The 
user can choose to pick 2-4 characters by checking the check boxes under the portraits. 

The numbers in the location can be inspected by clicking on them. On the bottom right corner of the window will 
be the portrait of the character currently being used. When the player clicks on the portrait, it will bring up 
a drop down menu of actions to take. This menu shows the health points, inventory contents, several 
actions the player can choose, and locations to access. The location menu item is another drop down menu 
containing all possible locations. The visibility of these locations will be initially false and will be turned to 
true throughout progress of the game. When a location is selected, the form will change the location and provide 
different location numbers to click on.