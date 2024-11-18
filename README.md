## VLSI SKILL ASSESSMENT 

## RIPPLE CARRY ADDER Design and Implementation using Cadence EDA Tools

## Abstract
To design and implement a Ripple carry adder circuit using Cadence EDA tools, simulate its functionality, and analyze key parameters such as gain, input impedance, output impedance, and frequency response, helping to understand its behavior in impedance matching and voltage buffering applications.

## Circuit Design
![digital_Logic2](https://github.com/user-attachments/assets/bf63ed76-1a5d-4c9b-9b61-822f894dfbcc)

## Circuit Description
A Ripple Carry Adder (RCA) is a basic digital circuit used for adding two multi-bit binary numbers. It consists of a cascade of full adders, each responsible for adding one bit from the input numbers and carrying the overflow to the next bit position. The goal of this assignment is to create the circuit schematic, perform simulations, and analyze its voltage gain, input/output impedance, and signal behavior under different input conditions.

## Getting Started Setting Up Cadence Virtuoso Open Terminal:

Right-click and open the terminal window. Enter the following commands: sh Copy code csh source /cadence/install/cshrc virtuoso

## Creating New Library & Schematic:

Library: File -> New -> Library, name it (e.g., VLSILAB_EXP_2), and attach it to the technology library gpdk045. Schematic Cell View: Go to File -> New -> Cell View, set up the library, cell, and view as follows: Library: Select your created library. Cell Name: E.g., Common_drain. View: Schematic. Adding Components and Connections:

Use the instance tool to add components such as nmos1v and pmos1v. Add input and output pins, and make all connections using the wire tool.
![Screenshot(37) 2024-11-18 at 7 33 25 PM (1)](https://github.com/user-attachments/assets/23cab29b-6d34-4bfb-b32b-27d4dfa17c16)


## Symbol Creation:

Go to Create -> Cell View -> From Cell View to generate the symbol automatically. Customize the symbol if needed. Simulation with Spectre Set Up Simulation: 

Use symbol to make circuit 
![Screenshot(38) 2024-11-18 at 7 33 26 PM](https://github.com/user-attachments/assets/1dc91571-8261-4e60-97f2-adc835fcd273)

Launch ADE L (Analog Design Environment). Set the simulation to Spectre and configure settings in Setup -> Simulation Directory/Host. 
Use Analysis -> Choose to configure settings for DC sweep or AC sweep or transient
Simulate the Common Drain Amplifier circuit.

## Results of simulation
After simulation, verify the expected characteristics of the common drain amplifier. The simulation should demonstrate the following:
High Input Impedance: Verify minimal loading on the signal source.
Low Output Impedance: Confirm efficient driving capability for subsequent stages.
Unity Voltage Gain (or Slightly Less): Ensure the output voltage closely follows the input signal.

![Screenshot(39) 2024-11-18 at 7 33 26 PM (1)](https://github.com/user-attachments/assets/028399b8-9206-4f04-b77b-6cfa1c6c82ba)



## Conclusion
The design and simulation of the Ripple carry adder using Cadence EDA tools were successful, confirming its impedance buffering properties and suitability for applications requiring high input impedance and low output impedance.
