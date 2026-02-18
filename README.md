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
- Threhold Voltage (Vt) is the gate voltage,when grounded all termimals, starting from zero, and gradully increasing postively, until it reaches minimum volatage required to form a conductive channel between the source and drain to turn on the NMOS.
- It is a function of x,y,z. which can accurately describes the NMOS Transistor. Here we called as Models.
- ## Modeling of Threshold Volatage
- Let, consider Vgs=0
- Source, Connect Drain, and Body to GND
- Now, Source-Body and Drain-Body acts as a pn junction diode
- As both junctions are OFF, there is a huge resistance between Source and Drain, thus no conductivity between Source and Drain.
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/20b7652d-1b59-42d7-bfcc-6b73ef21a153" /> <br>

- When a small positive voltage is applied to the gate, an electric field is established across the gate oxide.
- Then the gate oxide acts as a capacitor, causing repells the holes(postive charges) in the p-type substrate deeper into the substrate, leaving behind immobile negative ions near the surface.
- As the negative charges are accumulate near to the gate oxided, a depletion region forms (depleting the majority charge carries) inside the NMOS near to the surface.
   
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/814aeeb1-24a2-4507-81fb-25d131c3f4ae" />

# L3: Strong inversion and threshold voltage
- We can also state the threshold voltage as the Vgs voltage at which 'strong inversion' occurs  is called Threshold Voltage(Vt).
- Further increase in the Gate potential, there is no change in the Depletion layer width, but the channel width is increases by attracting the electrons from the  heavily doped 'n+' source region.
- In order to decides the thershold voltage equation. we have to consider the body terminal.

<img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/4fe867eb-148a-47aa-90a4-052ea7cd70bd" />
- by applying Vsb = 0 (left side)
- by applying Vsb = +ve value (right side), depletion width will be more at source side be

<img width="600" height="371" alt="image" src="https://github.com/user-attachments/assets/8ff3157a-0861-4dee-8388-0a73fa2e137f" />

<img width="600" height="373" alt="image" src="https://github.com/user-attachments/assets/873e3efb-05cf-4135-b877-3da90caf3497" />

- Applying a positive voltage to the substrate, an additional reverse bias is observed, as the source is now more negatively charged and the substrate is positively charged.
- This increases the depletion layer width more near the source.

<img width="600" height="402" alt="image" src="https://github.com/user-attachments/assets/1c6dd5ab-c502-4f76-9a7b-4f70096b723a" />

# L4: Threshold voltage with positive substrate potential

- On left side(Vbs = 0), there is the surface inversion takes places. 
- Semiconductor surface inverts to n-type material at voltage Vgs = Vto

<img width="890" height="431" alt="image" src="https://github.com/user-attachments/assets/e8d15ecc-87b5-4408-b3dd-fc8665361189" />

- On right Side(Vbs = +ve value), there is the less surface inversion takes place becasue of few charges are pulled towards source.
- An additional voltage (say V1) is required to overcome the increased depletion charge.
- At some potential,  Semiconductor surface inverts to n-type material at voltage Vgs = Vto + V1 
- from both of the cases, we have to concluded that in presence of substrate bias 'Vsb', additional potential is required for strong inversion.

<img width="440" height="176" alt="image" src="https://github.com/user-attachments/assets/8e548b49-710d-448e-9fc3-8268be332791" />

<img width="361" height="256" alt="image" src="https://github.com/user-attachments/assets/d14a1439-d6e6-4569-b071-61841bdd42c7" />

- These values are obtained from the foundry and fed into the SPICE model for device modelling and simulation.





