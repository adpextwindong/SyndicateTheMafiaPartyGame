SyndicateTheMafiaPartyGame
==========================

CS 5-6 2nd Semester Project

Our take on the party game Mafia
Design Doc
Team:
Gabe
Aidan
Takumi

Formal Game Description:

-The game starts out with a blank console window
-Each player is secretly assigned a role
-Roles include Inspector, Nurse, Criminal, and Voodoo Doctor
  -Inspectors choose a target player and can see who uses their ability on them during the night but not what that ability is.
	-Nurses choose a target player and prevents them from dying on the night.
	-Criminals choose a target player to kill during the night.
	-Voodoo Doctors choose a target player to curse that night and they die during the next
 night.
-After each player has been assigned a role, the game moves on to an augmented day phase
	Augmented Day Phase
		-Lasts 30 seconds
		-Players may chat freely
		-A regular night phase begins after
	Regular Night Phase
		-Lasts 30 seconds
		-Players may use their role's ability
		-At the end of the 30 seconds all of the abilities are executed
		-A regular day phase begins after
	Regular Day Phase
		-Lasts 2 minutes
		-Players may chat freely for 30 seconds
		-Players vote on a player to put up to trial for 30 seconds
		-If a player receives a majority of votes, he is put up to trial
		-If not the day phase ends
		-If there is a trial then the player has 30 seconds to make a defense
		-After the defense players have 30 seconds to vote if they are guilty or innocent
		-If they are guilty they are executed and the day ends
		-If they are innocent they are let free and the day ends
		-Once day ends a Regular Night Phase begins

Special Rules:
-Inspectors can't tell who the Voodoo Doctor visits
-If the Voodoo Doctor dies before the curse kills their target, the curse expires
-Doctor has to heal the person on the night the curse activates to prevent their death, not the night they are cursed.
-Criminal cannot kill the Voodoo Doctor
-Only one Criminal
-Only one Nurse
-Only one Voodoo Doctor
-Remaining players are inspectors
-6-10 players recommended

Formal Declaration:
Our project is our interpretation of the party game Mafia. This project will involve client-server design, networking (websockets) and server end multithreading/concurrency for gamestate maintenance. The initial goal is to have basic implementation of the game. This includes connection, initialization and chat for affecting gamestate later on with valid commands. For later implementation some goals for example will be a complete graphical display with a much less text based game and much more emphasis on graphics.

Goals:
Server Side set up - 3/16
Client Side set up - 3/30
Global Chat System between players - 4/6
Augmented Day Sequence - 4/13
Regular Night Sequence - 4/20
Regular Day Sequence - 4/27
Full text based game - 5/4
Basic Graphical Display - 5/24
Interface - 6/8
Complete game finished - 6/15

Extra Goals:
Game Saves
Spectator (Through Player type in Player Class)
Audio Assets
Chat Log, player vision syntax
Replays

Resources:
http://docs.oracle.com/javase/tutorial/essential/concurrency/index.html
http://docs.oracle.com/javase/tutorial/networking/sockets/index.html
