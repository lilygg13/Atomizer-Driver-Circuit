# Atomizer-Driver-Circuit
This project details the function of and improvements made upon the atomizer driver circuit for the levitated diamond experiment in Dutt Lab. 

The original circuit design is found in Jen-Feng Hsu's thesis in Section E.1. A schematic is shown below.

<img width="447" alt="Screenshot 2024-04-12 at 12 27 47 PM" src="https://github.com/user-attachments/assets/0a18d70b-7358-44af-9ae6-c1d001b84219">

Important parameters listed in the thesis are for the Arduino to send out switching signals sweeping from 150 kHz to 200 kHz in order to hit the resonant frequency of the horn and for S1 to be set to 30 V in order to generate droplets of the DBS and nanodiamond slurry.

In this project, the Arduino DUE is replaced with only the ATmega38P chip and a 16 MHz crysal oscillator. Details on how to wire and program the chip using an AVR pocket programmer are found at this link - https://www.allaboutcircuits.com/projects/atmega328p-fuse-bits-and-an-external-crystal-oscillator/. It is also possible to program the chip using a full Ardunio UNO board instaed of the pocket programmer (the ATmega chip pops out of the UNO board easily).

Additionally, the 15 V power supply S2 is replaced with a LM7815CT voltage regulator. This eliminates the need for any power source other than S1 from a DC power supply.

An updated schematic is shown below.

<img width="960" alt="Screenshot 2024-08-19 at 3 52 59 PM" src="https://github.com/user-attachments/assets/2ada5ecf-f1c2-4481-a5fe-24b13e4ce07f">


