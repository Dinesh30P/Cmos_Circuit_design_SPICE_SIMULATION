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
- We can also state that the threshold voltage as the Vgs voltage at which 'strong inversion' occurs  is called Threshold Voltage(Vt).
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

- On the left side(Vbs = 0), there is the surface inversion takes places. 
- Semiconductor surface inverts to n-type material at voltage Vgs = Vto

<img width="890" height="431" alt="image" src="https://github.com/user-attachments/assets/e8d15ecc-87b5-4408-b3dd-fc8665361189" />

- On the right Side(Vbs = +ve value), there is the less surface inversion takes place becasue of few charges are pulled towards source.
- An additional voltage (say V1) is required to overcome the increased depletion charge.
- At some potential,  Semiconductor surface inverts to n-type material at voltage Vgs = Vto + V1 
- from both of the cases, we have to concluded that in presence of substrate bias 'Vsb', additional potential is required for strong inversion.

<img width="440" height="176" alt="image" src="https://github.com/user-attachments/assets/8e548b49-710d-448e-9fc3-8268be332791" />

<img width="361" height="256" alt="image" src="https://github.com/user-attachments/assets/d14a1439-d6e6-4569-b071-61841bdd42c7" />

- These values are obtained from the foundry and fed into the SPICE model for device modelling and simulation.

# L1: Resistive region of operation with small drain-source voltage
## Resistive Operation
- Vgs is increases then channel width is increases, becauses of the induced charges casued by the gate voltage

<img width="600" height="349" alt="image" src="https://github.com/user-attachments/assets/e0472695-f013-4799-a17d-214e7a7f9368" />

- Lets, consider Vgs = 1V,
- Vds = 0.05V
- Vt = 0.45V
- Qi ∝ (Vgs-Vt)
- There is voltage gradient throughout the channel which starts at zero and at Vds 
- Here, X-axis represents the channel length and Y-axis represents the channel width
- V(x) is the Voltage at a point 'x' along channel 

<img width="539" height="439" alt="image" src="https://github.com/user-attachments/assets/fd6929e7-76e6-41c5-9226-3439e1136fcf" />

- Gate to channel Voltage at that point on the application of Vds is Vgs-V(x)

# L2: Drift current theory
- Now, in the channel, induced at any point
- Qi(x) ∝ ([Vgs-V(x)]-Vt)
- i.e Qi(x) = -Cox([Vgs-V(x)]-Vt)
- here Cox is the Gate oxide capcitance  
-  Cox = εox / tox
-  εox is Oxide permittivity = 3.97x εo(Relative permittivity)
-  3.5 x 10e-11 F/m
-  tox = oxide thickness
  
-<img width="844" height="421" alt="image" src="https://github.com/user-attachments/assets/3a5d414e-b6f1-442d-a597-5a3c8086d5db" />

- Drift current is been measured as velocity of the charge carriers multipiled by avaliable charges over the channel width (complete area).

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/8fc1d9ef-6b84-47ea-9654-cf3de1290af4" />

# L3: Drain current model for linear region of operation

- velocity is Vn(x), W is width, mobility of the carriers and electric field

<img width="292" height="410" alt="image" src="https://github.com/user-attachments/assets/a85ac293-afbd-4ead-aa22-1382629a3d76" />

- Substituing and Intergrating dx over channel lenght L will give the V-I relation of NMOS transistor.

<img width="315" height="327" alt="image" src="https://github.com/user-attachments/assets/e0ff3e90-7c15-44f2-88f7-36576ca0c9b6" />

- when ever (Vds <= Vgs-Vt) MOSFET operates in the linear region.

## Current Equation for Linear Region 

Id = (Kn)*{(Vgs-Vt)Vds - Vds**2 / 2} 
  
<img width="503" height="306" alt="image" src="https://github.com/user-attachments/assets/b955d07a-bbea-4164-a6ef-946645add5c3" />
# L4: SPICE conclusion to resistive operation

- For linear region operation we have to make sure that  (Vds <= Vgs-Vt) so we neglection the 
Vds^2 / 2 term in the current equation.

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/31b06dbb-93c9-46de-a840-4eb047d1a460" />

- here we have sweep the values of Vds ranging for 0 to 2.05 but maintaining the condition         Vds <= Vgs-Vt to be in the linear region or restitve region of operation.
- if Vds >= Vgs-Vt then device enters into the saturation region

# L5 Pinch-off region condition

- if Vds >= Vgs-Vt then device enters into the saturation region
- Vgs- V(x) is the gate to channel volatage at that point
- channel voltage = =Vgs-Vds

<img width="522" height="415" alt="image" src="https://github.com/user-attachments/assets/ae00abbf-81fc-4570-bcae-0eea0a64d1de" />



| Vgs | Vds  | Vgs - Vds |   | Vt   |
|-----|------|-----------|---|------|
| 1   | 0.05 | 0.95      | > | 0.45 |
| 1   | 0.15 | 0.85      | > | 0.45 |
| 1   | 0.25 | 0.75      | > | 0.45 |
| 1   | 0.35 | 0.65      | > | 0.45 |
| 1   | 0.45 | 0.55      | > | 0.45 |
| 1   | 0.55 | 0.45      | = | 0.45 |
| 1   | 0.65 | 0.35      | < | 0.45 |
| 1   | 0.75 | 0.25      | < | 0.45 |
| 1   | 0.85 | 0.15      | < | 0.45 |
| 1   | 0.95 | 0.05      | < | 0.45 |

- At Vgs > Vt (surface inversion already happens)
## Pinch of Phenomenon Started
- i.e channel begins to disappear(linearity of the current flow changes)
- At this point Vt = Vgs-Vds(surface iversion just happens / about to happen )

<img width="504" height="432" alt="image" src="https://github.com/user-attachments/assets/d197b2b5-2be4-44da-958c-e235c6dcfd13" />

 ## Pinch off Region

-  here Vgs-Vds < Vt(no channel present near to the drain)
 
-  <img width="500" height="444" alt="image" src="https://github.com/user-attachments/assets/685c7cf4-2b31-4383-87a7-d2d95e2d91cd" />

# L6: Drain current model for saturation region of operation

- Voltage over the channel remains constant  = Vgs-Vt (Vds is negligible/ vanished)
- In the current Equation Vds in the channel voltage{Vgs- Vds} is Replace by (Vgs-Vt)
- Then the equation turns into (no more linear function of f(Vds))

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/362d136e-9a9a-48c9-97f3-19ebfe1ae079" />

- Even it look like perfect current source i.e current is constant, but it is not 'correct'
- Due to effective conductive channel length is modualated by applied Vds
- Even it going to reduces if Vds further increase
- For getting more accurate equation, and (λ * Vds) is added
- Here, λ = Channel length modulation

<img width="500" height="304" alt="image" src="https://github.com/user-attachments/assets/e0a9cd88-07fe-4b8b-8e6d-82ee22999f5a" />

## Constant Current Equation for Saturation Region 

- Id = (Kn'/2)(W/L)(1+ λ*Vds)(Vgs-Vt)**2

# L1 Basic SPICE setup

- It is basically a software and its an engine which can derives some waveform by giving inputs
- This waveforms are used to calculate the delay of the cell
- This delays are accurate and used to Static Timing Analysis(STA)

##  SPICE Model Parameters 
- The highlighted ones are the constants will come from the foundaries when we tackle advance technology nodes

<img width="612" height="421" alt="image" src="https://github.com/user-attachments/assets/eb44d327-72f0-4f90-8070-435ce1113d0e" />

## SPICE setup Flow chart

<img width="426" height="491" alt="image" src="https://github.com/user-attachments/assets/b60bbe86-2c9a-4c0b-9ed6-22a0167b0837" />

## Spice Netlist 
- A SPICE netlist is a plain text file that defines the components and connections of an electronic circuit, allowing it to be analyzed and simulated using SPICE software.

<img width="783" height="396" alt="image" src="https://github.com/user-attachments/assets/088e3d30-d3eb-455e-9a0b-fa1683dce2c4" />

# L2: Circuit description in SPICE syntax

- let's give the values for the netlist
- Here, We can considering 4 nodes (where there is no obstraction we can consider as node)

<img width="437" height="372" alt="image" src="https://github.com/user-attachments/assets/3998d2e2-e461-4278-9b9f-3169d6be1a5a" />

- In an electrical circuit, a node is a point where two or more components are connected together. It represents a location where the electrical potential (voltage) is the same for all connected elements.
- Nodes are used in circuit analysis to determine voltages and currents throughout the system.

  ## DGSS
  
<img width="806" height="309" alt="image" src="https://github.com/user-attachments/assets/7da08862-1bc6-4461-a3c7-9d434fcc8125" />

- MOSFET have 4 terminals i.e Drain, Gate, Source, Substrate/Bulk
### For the First Component (MOSFET)
- M1 --> MOSFETXX (XX- number), Vdd --> Drain, 0 --> Source node, 0 --> Substrate node, NMOS --> it comes from technology file, W= 1.8µ --> Width of the Gate in microns, L = 1.2µ --> length of the Gate in Micron.

 ### For the Second Componet (Resistor)
 - R1 --> ResistorXX (XX- number), in --> First terminal, n1 --> Node 1 {R1 is between in and n1}, 55 Ω --> Resistance  Value in Ohms

### Vdd Source 
- VXX --> Voltage source XX(it will between 2 nodes i.e Vdd and Zero), here  Vdd is 2.5 Volts.
- Vin lies in between in(postive terminal)and Zero (negative terminal), here  Vin is 2.5 Volts.

- Once we define the netlist, next we have to define the technology file.

<img width="420" height="200" alt="image" src="https://github.com/user-attachments/assets/4bd4c5c2-375c-48c6-8573-4312ff961239" />


  # L3: Define Technology Parameters
 
## Models
 - AND gate is a BOOLEAN Multiplication of two inputs
 - OR gate is a BOOLEAN Addition of two inputs

## For Model Files(Vt,Id...) --> Model Parameters(γ, kn'/2...) are Required

<img width="839" height="444" alt="image" src="https://github.com/user-attachments/assets/163ce3ae-2771-45a8-bcf2-1ffe17f7e2b2" />

- for Nmos model file we have to choose NMOS package (its very important)

<img width="471" height="393" alt="image" src="https://github.com/user-attachments/assets/8cacb959-fbbd-408b-8e41-cfbc1df79ad0" />

### Package in a file (.mod )

### .LIB "xxxx_025µm_model.mod" CMOS_MODELS

### Simulation commands
- We have to Sweep Drain and Gate Voltage

<img width="690" height="470" alt="image" src="https://github.com/user-attachments/assets/4f64cabc-50ae-41a2-b857-92f23dda6bfc" />

# L4: First SPICE simulation






   












  












  













