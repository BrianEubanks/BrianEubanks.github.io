---
layout: post
title:  "Chip 8 Simulator"
date:   2020-11-22 11:44:40 -0600
categories: projects
project: CS
---

{:refdef: style="text-align: center;"}
#### CHIP 8 Simulator - IBMLOGO
{: refdef}
{:refdef: style="text-align: center;"}
![bship1](/images/chip8/chip8IBM.png)
{: refdef}

I'm currently in the process of building a [CHIP8 simulator] in Python and Java. Currently the Python version only shows the display output, whereas the Java version also shows the memory and register contents. The IBMLogo rom loads by default if no file is specified at runtime.  *So far only the Instructions needed for the IBMLogo are implemented so other roms may not run too well!*

[Chip8] is a simple virtual machine with a simple architecture, making it an easy starting point for writing simulators and emulators. There are many resources and references online, so for now I won't go into great details on the instruction set.

#### Future Work

Implement the remaining instructions and test with some other roms.

Finish Java simulator. Add Save/Load states. Live memory editing. Rom Editing.

Move on to implement other architectures and older video games systems.

Write an Arduino Simulator. I found some generic AVR simulators in addition to the built in debugger with Atmel studio, however I think a more robust simulator could be useful. Particularly having the ability to simulate external interrupts and some basic hardware peripherals.







[Chip8]: https://en.wikipedia.org/wiki/CHIP-8
[CHIP8 simulator]: https://github.com/BrianEubanks/chip8

