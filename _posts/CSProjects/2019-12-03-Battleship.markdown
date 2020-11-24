---
layout: post
title:  "Battleship"
date:   2019-12-03 16:00:00 -0600
categories: projects
project: CS
---
This [Battleship] was a senior capstone group project for our Sofware Engineering class written in Java. The game is hosted on a server and clients connect and login to play.

{:refdef: style="text-align: center;"}
#### Start Screen
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/bship/bship1.png)
{: refdef}

{:refdef: style="text-align: center;"}
Start screen for two clients connected to the server on localhost.
{: refdef}



### Current State

In order to play, a SQL server must be setup. The scripts to initialize the user tables are included in the repository. The tables store user data, and the players must create an account to login and play.

The BattleshipServer connects to the database and listens for client connections.

When two BattleshipClients connect to the server the game begins! 

{:refdef: style="text-align: center;"}
#### Login
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/bship/bshipClientServer.png)
{: refdef}
{:refdef: style="text-align: center;"}
Left: Local Server Window. Right: Client connect to server with login prompt.
{: refdef}

{:refdef: style="text-align: center;"}
#### Placing Ships
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/bship/bship2.png)
{: refdef}

{:refdef: style="text-align: center;"}
#### Gameplay
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/bship/bship4.png)
{: refdef}
{:refdef: style="text-align: center;"}
Gameplay. Players click on the top half to guess where their opponents ships are.
{: refdef}

{:refdef: style="text-align: center;"}
#### Game Over
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/bship/bship3.png)
{: refdef}




### Future Work

This could be modified to create a local only version.

The Login process could be more aesthetic. It's a little clunky, and would need to be more eyecatching and user friendly if it were to be ported to a true app.

Implement customizable game parameters, like the number of ships, size of the ships, the size of the board, etc...

Create a Chess or Backgammon game!


[Battleship]: https://github.com/BrianEubanks/Battleship


