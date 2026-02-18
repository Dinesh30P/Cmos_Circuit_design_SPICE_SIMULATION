# CMOS_Circuit_design_&_SPICE_SIMULATION
 
# L1: Why is SPICE Simulation needed?
- To verify circuit behavior before fabrication
-  To optimize the Performance
-  To reduce the Cost and improve timing efficiency

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d0cd4084-6e16-4550-97e7-6f5c899e44ce" />


## What is circuit design and SPICE?
- circuit design consists of logic gates AND,OR,NOT,Buffer...made up of PMOS and NMOS transistors connected in particular fasion
- SPICE is a Simulation Program with Integrated Circuit Emphasis, which genereats the waveform defines the delay of the pariticlar cell based on the waveform shape.

## Why do we need SPICE?
- The clocktree synthesis, timing, crosstalks are build on the SPICE, without having SPICE there won't be delays and if there is no delays physical design flow, crosstalk won't make any sense.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/ea9a8b75-a1f8-4b46-9179-3cd58b61fc3f" />

## clocktree sysnthesis
- delay table consists of  i/p slew and o/p load for buffer types (level 1, level 2)
- intersection value consider as the delay
- if the delay table not provide any value then we have to do interpolation between two values through equations
- Each transistor (PMOS & NMOS) is unique, with different delay values and buffer sizing (W & L) delay behavior and determines current.
- Buffer differentiation is part of circuit design.
- Length(L) and  Width(W)  decide the Drive current (I) and the resulting timing curve

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/caded01a-8ef3-44c6-adc9-2f13e7e38b9a" />

- 
