# CS-350 Emerging Systems Architecture and Technology

This repo documents my work for CS-350 at Southern New Hampshire University. The course covers hands-on hardware and software work with a Raspberry Pi, including setup, wiring, state machines, and a final thermostat project.

## Contents
- [Thermostat.py](./Thermostat.py): Final project. A smart thermostat prototype with a state machine, three buttons, an AHT20 temperature sensor, LEDs, an LCD, and UART output
- [Milestone3.py](./Milestone3.py): Morse code project that flashes SOS and OK with LEDs, with a button to switch messages, LCD feedback, and a graceful exit
- [module-1-pi-setup](./module-1-pi-setup): Setting up the Raspberry Pi lab environment and connecting over SSH

## Tools and technologies
Raspberry Pi running Ubuntu 24.04, SSH, Python, GPIO, I2C, UART

## Project Reflection

**Summarize the project and what problem it was solving.**
For my final project I built a smart thermostat prototype on a Raspberry Pi. It reads room temperature from an AHT20 sensor, shows information on an LCD, and uses LEDs to show whether the system is heating, cooling, or off. A state machine controls how it moves between modes, and three buttons let the user change the mode and raise or lower the temperature setpoint. It also sends a status message over UART every 30 seconds. The problem it solves is giving a user a simple, automatic way to keep a space at a set temperature. My Milestone 3 project, the Morse code program, was an earlier step that used the same state machine ideas.

**What did you do particularly well?**
I planned before I coded. I spent time understanding the requirements and mapping out the state machine first, which made the code easier to write. I also tested each part of the hardware on its own before putting everything together, which helped me find problems faster.

**Where could you improve?**
Debugging took longer than I expected, especially when I combined multiple components. At one point the sensor threw errors because two parts of the program were reading it at the same time, and a button did not work because of a missing ground wire. I could improve by writing small tests earlier and keeping better notes on what I tried.

**What tools and/or resources are you adding to your support network?**
The course materials and zyBooks, the official documentation for the Raspberry Pi and its Python libraries, GitHub for documenting my work, draw.io for state machine diagrams, and my instructor and classmates in the discussion boards.

**What skills from this project will be particularly transferable to other projects and/or course work?**
Breaking a big problem into smaller parts, testing one piece at a time, reading hardware documentation, and using a state machine to organize logic. These apply to any project that mixes software and hardware, and to troubleshooting in general.

**How did you make this project maintainable, readable, and adaptable?**
I used clear names for variables and functions and added comments to explain the reasoning behind my choices. I kept the state machine logic organized so I could change a mode or setting without rewriting everything, and I made a state machine diagram that matches the code, so the design is easy to follow later.

## About me
I'm a software engineering student at SNHU, graduating in April 2027. This portfolio is where I document what I build and what I learn along the way.
