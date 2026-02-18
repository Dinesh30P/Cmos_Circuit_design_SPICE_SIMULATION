# CMOS_Circuit_design_&_SPICE_SIMULATION
 
# L1: Why is SPICE Simulation needed?
- To verify circuit behavior before fabrication.
-  To optimize the Performance.
-  To reduce the Cost and improve timing efficiency.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d0cd4084-6e16-4550-97e7-6f5c899e44ce" />


## What is circuit design and SPICE?
- circuit design consists of logic gates AND,OR,NOT,Buffer...made up of PMOS and NMOS transistors connected in particular fasion.
- SPICE is a Simulation Program with Integrated Circuit Emphasis, which genereats the waveform defines the delay of the pariticlar cell based on the waveform shape.

## Why do we need SPICE?
- The clocktree synthesis, timing, crosstalks are build on the SPICE, without having SPICE there won't be delays and if there is no delays physical design flow, crosstalk won't make any sense.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/ea9a8b75-a1f8-4b46-9179-3cd58b61fc3f" />

## Clocktree sysnthesis
- delay table consists of  i/p slew and o/p load for buffer types (level 1, level 2)
- intersection value consider as the delay
- if the delay table not provide any value then we have to do interpolation between two values through equations
- Each transistor (PMOS & NMOS) is unique, with different delay values and buffer sizing (W & L) delay behavior and determines current.
- Buffer differentiation is part of circuit design.
- Length(L) and  Width(W)  decide the Drive current (I) that results in the timing curves.

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/caded01a-8ef3-44c6-adc9-2f13e7e38b9a" />

# L2: Introduction to basic element in Circuit design – NMOS

A transistor is a semiconductor device that can control the current flow through an electric field and functions mainly as an amplifier or a switch. The MOS transistor is the core device mostly used in CMOS circuits. A MOS transistor can be either n-type (NMOS) or p-type (PMOS) depending on the doping and dominant charge carriers.

|Component          | Description        |     Key Notes                    |
|---------------------------|--------------------|--------------------------------------------------------|
|P‑type Substrate      | Base semiconductor foundation                   | - Serves as the body  <br> - Provides holes as majority carriers |
| Isolation Region | Areas separating nearby devices | - Prevents electrical interaction <br> - Reduces leakage and latch‑up risks |
| Gate Oxide | Thin insulating layer above substrate | - Commonly SiO₂ <br> - Governs channel creation <br> - Influences threshold voltage |
| Polysilicon / Metal Gate | Conductive layer placed over gate oxide| - Acts as the Gate terminal <br> - Controls channel via electric field <br> -Enables switching |
| Body Terminal | Substrate connection point | - Often grounded in NMOS <br> - Impacts threshold voltage (body effect) <br> - Important for modeling |

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/ee5ea8b2-ae84-4e63-8b09-3ab224b7b79d" />

## Threshold Voltage:
- Threhold Voltage (Vt) is the Gate Voltage
- It is a function of x,y,z. which can accurately describes the NMOS Transistor. Here we called as Models.
- <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/20b7652d-1b59-42d7-bfcc-6b73ef21a153" />
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/814aeeb1-24a2-4507-81fb-25d131c3f4ae" />


