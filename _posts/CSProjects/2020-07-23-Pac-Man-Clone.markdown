---
layout: post
title:  "Pac-Man Clone"
date:   2020-7-23 11:44:40 -0600
categories: projects
project: CS
---
This [Pacman] clone started as a small Covid side project until my research project and other work projects took higher priority. I wanted to create a clone that ran as close as possible to the original. The [Pacman Dossier] served as a valuable reference to some of the little quirks and intricacies.

{:refdef: style="text-align: center;"}
#### Start Screen
{: refdef}
{:refdef: style="text-align: center;"}
![Pacman01](/images/pacman01.png)
{: refdef}


### Current State

One level can kind of be played. As soon as the board is cleared, it immediately resets the board, and slightly increases the speed of the ghost and pacman. And the power dots don't work :(

Currently it uses an SDL library to handle the graphics. The map tiles and character sprites are pixel perfect to the original. Blinky appears upside down because it uses the same drawing method as Pacman. The Pacman sprite is rotated depending on the direction, so the Blinky sprite is rotated as well.

The 'ugly' squares on the screenshot mark intersections. These are squares that the ghosts must make a decision on which direction to turn, based on it's direction and the location of it's target squared. Some things to keep in mind is that it cannot perform a 180 turn at any intersection, and it cannot turn 'UP' at the intersections in the middle, the ones right between the ghost and pacman starting positions. They have a slightly different 'ugly' tile sprite.


Currently only Blinky is implemented. He has a target square (one square in front of pacman) that he always travels towards, obeying the intersection rules. It is not 100% yet, as sometimes he will sneak outside of the maze when traveling through the tunnels on the edges. Once this bug is fixed I can add the other ghosts in. The only difference in their behavior is their target squares.

### Future Work

This C version may or may not get finished. Maybe it would be better to do C++ and get a crossplatform makefile working.

I might instead implement this in Java along with a map editor, or maybe just the map editor!

I would be interested in implementing a full emulator to just run the original Rom file, or perhaps implementing the PacMan board on FPGA!




[Pacman]: https://github.com/BrianEubanks/Pacman
[Pacman Dossier]:  https://github.com/jekyll/jekyll

