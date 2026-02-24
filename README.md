# NNgspiceSky130 - Day 1 - Basics of NMOS Drain current (Id) vs Drain-to-source Voltage (Vds)

## Introduction to Circuit Design and SPICE simulations

### CMOS_Circuit_design_&_SPICE_SIMULATION
 
#### L1: Why is SPICE Simulation needed?
- To verify circuit behavior before fabrication.
-  To optimize the Performance.
-  To reduce the Cost and improve timing efficiency.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/d0cd4084-6e16-4550-97e7-6f5c899e44ce" />


###### What is circuit design and SPICE?
- circuit design consists of logic gates AND,OR,NOT,Buffer...made up of PMOS and NMOS transistors connected in particular fasion.
- SPICE is a Simulation Program with Integrated Circuit Emphasis, which genereats the waveform defines the delay of the pariticlar cell based on the waveform shape.

###### Why do we need SPICE?
- The clocktree synthesis, timing, crosstalks are build on the SPICE, without having SPICE there won't be delays and if there is no delays physical design flow, crosstalk won't make any sense.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/ea9a8b75-a1f8-4b46-9179-3cd58b61fc3f" />

###### Clocktree sysnthesis
- delay table consists of  i/p slew and o/p load for buffer types (level 1, level 2)
- intersection value consider as the delay
- if the delay table not provide any value then we have to do interpolation between two values through equations
- Each transistor (PMOS & NMOS) is unique, with different delay values and buffer sizing (W & L) delay behavior and determines current.
- Buffer differentiation is part of circuit design.
- Length(L) and  Width(W)  decide the Drive current (I) that results in the timing curves.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/caded01a-8ef3-44c6-adc9-2f13e7e38b9a" />

#### L2: Introduction to basic element in Circuit design – NMOS

A transistor is a semiconductor device that can control the current flow through an electric field and functions mainly as an amplifier or a switch. The MOS transistor is the core device mostly used in CMOS circuits. A MOS transistor can be either n-type (NMOS) or p-type (PMOS) depending on the doping and dominant charge carriers.

|Component          | Description        |     Key Notes                    |
|---------------------------|--------------------|--------------------------------------------------------|
|P‑type Substrate      | Base semiconductor foundation                   | - Serves as the body  <br> - Provides holes as majority carriers |
| Isolation Region | Areas separating nearby devices | - Prevents electrical interaction <br> - Reduces leakage and latch‑up risks |
| Gate Oxide | Thin insulating layer above substrate | - Commonly SiO₂ <br> - Governs channel creation <br> - Influences threshold voltage |
| Polysilicon / Metal Gate | Conductive layer placed over gate oxide| - Acts as the Gate terminal <br> - Controls channel via electric field <br> -Enables switching |
| Body Terminal | Substrate connection point | - Often grounded in NMOS <br> - Impacts threshold voltage (body effect) <br> - Important for modeling |

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/ee5ea8b2-ae84-4e63-8b09-3ab224b7b79d" />

##### Threshold Voltage:
- Threhold Voltage (Vt) is the gate voltage,when grounded all termimals, starting from zero, and gradully increasing postively, until it reaches minimum volatage required to form a conductive channel between the source and drain to turn on the NMOS.
- It is a function of x,y,z. which can accurately describes the NMOS Transistor. Here we called as Models.
##### Modeling of Threshold Volatage

- Let, consider Vgs=0
- Source, Connect Drain, and Body to GND
- Now, Source-Body and Drain-Body acts as a pn junction diode
- As both junctions are OFF, there is a huge resistance between Source and Drain, thus no conductivity between Source and Drain.
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/20b7652d-1b59-42d7-bfcc-6b73ef21a153" /> <br>

- When a small positive voltage is applied to the gate, an electric field is established across the gate oxide.
- Then the gate oxide acts as a capacitor, causing repells the holes(postive charges) in the p-type substrate deeper into the substrate, leaving behind immobile negative ions near the surface.
- As the negative charges are accumulate near to the gate oxided, a depletion region forms (depleting the majority charge carries) inside the NMOS near to the surface.
   
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/814aeeb1-24a2-4507-81fb-25d131c3f4ae" />

#### L3: Strong inversion and threshold voltage
- We can also state that the threshold voltage as the Vgs voltage at which 'strong inversion' occurs  is called Threshold Voltage(Vt).
- Further increase in the Gate potential, there is no change in the Depletion layer width, but the channel width is increases by attracting the electrons from the  heavily doped 'n+' source region.
- In order to decides the thershold voltage equation. we have to consider the body terminal.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/4fe867eb-148a-47aa-90a4-052ea7cd70bd" />
- by applying Vsb = 0 (left side)
- by applying Vsb = +ve value (right side), depletion width will be more at source side be

<img width="500" height="401" alt="image" src="https://github.com/user-attachments/assets/8ff3157a-0861-4dee-8388-0a73fa2e137f" />

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/873e3efb-05cf-4135-b877-3da90caf3497" />

- Applying a positive voltage to the substrate, an additional reverse bias is observed, as the source is now more negatively charged and the substrate is positively charged.
- This increases the depletion layer width more near the source.

<img width="500" height="402" alt="image" src="https://github.com/user-attachments/assets/1c6dd5ab-c502-4f76-9a7b-4f70096b723a" />

#### L4: Threshold voltage with positive substrate potential

- On the left side(Vbs = 0), there is the surface inversion takes places. 
- Semiconductor surface inverts to n-type material at voltage Vgs = Vto

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/e8d15ecc-87b5-4408-b3dd-fc8665361189" />

- On the right Side(Vbs = +ve value), there is the less surface inversion takes place becasue of few charges are pulled towards source.
- An additional voltage (say V1) is required to overcome the increased depletion charge.
- At some potential,  Semiconductor surface inverts to n-type material at voltage Vgs = Vto + V1 
- from both of the cases, we have to concluded that in presence of substrate bias 'Vsb', additional potential is required for strong inversion.

<img width="400" height="306" alt="image" src="https://github.com/user-attachments/assets/8e548b49-710d-448e-9fc3-8268be332791" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/d14a1439-d6e6-4569-b071-61841bdd42c7" />

- These values are obtained from the foundry and fed into the SPICE model for device modelling and simulation.

### NMOS resistive region and saturation region of operation

#### L1: Resistive region of operation with small drain-source voltage

##### Resistive Operation
- Vgs is increases then channel width is increases, becauses of the induced charges casued by the gate voltage

<img width="500" height="409" alt="image" src="https://github.com/user-attachments/assets/e0472695-f013-4799-a17d-214e7a7f9368" />

- Lets, consider Vgs = 1V,
- Vds = 0.05V
- Vt = 0.45V
- Qi ∝ (Vgs-Vt)
- There is voltage gradient throughout the channel which starts at zero and at Vds 
- Here, X-axis represents the channel length and Y-axis represents the channel width
- V(x) is the Voltage at a point 'x' along channel 

<img width="509" height="4o9" alt="image" src="https://github.com/user-attachments/assets/fd6929e7-76e6-41c5-9226-3439e1136fcf" />

- Gate to channel Voltage at that point on the application of Vds is Vgs-V(x)

#### L2: Drift current theory
- Now, in the channel, induced at any point
- Qi(x) ∝ ([Vgs-V(x)]-Vt)
- i.e Qi(x) = -Cox([Vgs-V(x)]-Vt)
- here Cox is the Gate oxide capcitance  
-  Cox = εox / tox
-  εox is Oxide permittivity = 3.97x εo(Relative permittivity)
-  3.5 x 10e-11 F/m
-  tox = oxide thickness
   
-<img width="504" height="401" alt="image" src="https://github.com/user-attachments/assets/3a5d414e-b6f1-442d-a597-5a3c8086d5db" />

- Drift current is been measured as velocity of the charge carriers multipiled by avaliable charges over the channel width (complete area).

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/8fc1d9ef-6b84-47ea-9654-cf3de1290af4" />

#### L3: Drain current model for linear region of operation

- velocity is Vn(x), W is width, mobility of the carriers and electric field

<img width="400" height="310" alt="image" src="https://github.com/user-attachments/assets/a85ac293-afbd-4ead-aa22-1382629a3d76" />

- Substituing and Intergrating dx over channel lenght L will give the V-I relation of NMOS transistor.

<img width="405" height="307" alt="image" src="https://github.com/user-attachments/assets/e0ff3e90-7c15-44f2-88f7-36576ca0c9b6" />

- when ever (Vds <= Vgs-Vt) MOSFET operates in the linear region.

##### Current Equation for Linear Region 

Id = (Kn)*{(Vgs-Vt)Vds - Vds**2 / 2} 
  
<img width="503" height="406" alt="image" src="https://github.com/user-attachments/assets/b955d07a-bbea-4164-a6ef-946645add5c3" />
#### L4: SPICE conclusion to resistive operation

- For linear region operation we have to make sure that  (Vds <= Vgs-Vt) so we neglection the 
Vds^2 / 2 term in the current equation.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/31b06dbb-93c9-46de-a840-4eb047d1a460" />

- here we have sweep the values of Vds ranging for 0 to 2.05 but maintaining the condition         Vds <= Vgs-Vt to be in the linear region or restitve region of operation.
- if Vds >= Vgs-Vt then device enters into the saturation region

#### L5 Pinch-off region condition

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

<img width="504" height="402" alt="image" src="https://github.com/user-attachments/assets/d197b2b5-2be4-44da-958c-e235c6dcfd13" />

 ## Pinch off Region

-  here Vgs-Vds < Vt(no channel present near to the drain)
 
-  <img width="500" height="444" alt="image" src="https://github.com/user-attachments/assets/685c7cf4-2b31-4383-87a7-d2d95e2d91cd" />

#### L6: Drain current model for saturation region of operation

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

##### Constant Current Equation for Saturation Region 

- Id = (Kn'/2)(W/L)(1+ λ*Vds)(Vgs-Vt)**2

### Introduction to SPICE

#### L1 Basic SPICE setup

- It is basically a software and its an engine which can derives some waveform by giving inputs
- This waveforms are used to calculate the delay of the cell
- This delays are accurate and used to Static Timing Analysis(STA)

##### SPICE Model Parameters 
- The highlighted ones are the constants will come from the foundaries when we tackle advance technology nodes

<img width="512" height="321" alt="image" src="https://github.com/user-attachments/assets/eb44d327-72f0-4f90-8070-435ce1113d0e" />

##### SPICE setup Flow chart

<img width="506" height="401" alt="image" src="https://github.com/user-attachments/assets/b60bbe86-2c9a-4c0b-9ed6-22a0167b0837" />

##### Spice Netlist 
- A SPICE netlist is a plain text file that defines the components and connections of an electronic circuit, allowing it to be analyzed and simulated using SPICE software.

<img width="503" height="396" alt="image" src="https://github.com/user-attachments/assets/088e3d30-d3eb-455e-9a0b-fa1683dce2c4" />

#### L2: Circuit description in SPICE syntax

- let's give the values for the netlist
- Here, We can considering 4 nodes (where there is no obstraction we can consider as node)

<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/3998d2e2-e461-4278-9b9f-3169d6be1a5a" />

- In an electrical circuit, a node is a point where two or more components are connected together. It represents a location where the electrical potential (voltage) is the same for all connected elements.
- Nodes are used in circuit analysis to determine voltages and currents throughout the system.

##### DGSS
  
<img width="506" height="409" alt="image" src="https://github.com/user-attachments/assets/7da08862-1bc6-4461-a3c7-9d434fcc8125" />

- MOSFET have 4 terminals i.e Drain, Gate, Source, Substrate/Bulk
##### For the First Component (MOSFET)
- M1 --> MOSFETXX (XX- number), Vdd --> Drain, 0 --> Source node, 0 --> Substrate node, NMOS --> it comes from technology file, W= 1.8µ --> Width of the Gate in microns, L = 1.2µ --> length of the Gate in Micron.

##### For the Second Componet (Resistor)
- R1 --> ResistorXX (XX- number), in --> First terminal, n1 --> Node 1 {R1 is between in and n1}, 55 Ω --> Resistance  Value in Ohms

##### Vdd Source 
- VXX --> Voltage source XX(it will between 2 nodes i.e Vdd and Zero), here  Vdd is 2.5 Volts.
- Vin lies in between in(postive terminal)and Zero (negative terminal), here  Vin is 2.5 Volts.

- Once we define the netlist, next we have to define the technology file.

<img width="420" height="200" alt="image" src="https://github.com/user-attachments/assets/4bd4c5c2-375c-48c6-8573-4312ff961239" />


#### L3: Define Technology Parameters
 
##### Models
 - AND gate is a BOOLEAN Multiplication of two inputs
 - OR gate is a BOOLEAN Addition of two inputs

##### For Model Files(Vt,Id...) --> Model Parameters(γ, kn'/2...) are Required

<img width="539" height="404" alt="image" src="https://github.com/user-attachments/assets/163ce3ae-2771-45a8-bcf2-1ffe17f7e2b2" />

- for Nmos model file we have to choose NMOS package (its very important)

<img width="501" height="403" alt="image" src="https://github.com/user-attachments/assets/8cacb959-fbbd-408b-8e41-cfbc1df79ad0" />

##### Package in a file (.mod )

##### .LIB "xxxx_025µm_model.mod" CMOS_MODELS

##### Simulation commands
- We have to Sweep Drain and Gate Voltage

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/4f64cabc-50ae-41a2-b857-92f23dda6bfc" />

#### L4: First SPICE simulation

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5c808992-7f65-4902-9f58-f484d7ea67d5" />

- Id vs Vds Curve

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/a797f73a-b358-4fe5-9a6e-0a2187f2cb30" />

- Y-axis having Id in µA and X-axis is Vds in Volts
- we can get to observe different regions in the graph(cut off region on right bottom)which was ploted and we can see Vgs of different plot on right side(which was decreasing from top to bottom)

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/dc7248fb-5f46-4985-8fa1-fafc53617cf0" />


- We are sweeping with step of 0.2
- We are not observing any curve for Vgs = 0.2,0.4 i.e device should need to cross atleast thershold voltage.
- for this transistor we are consider a thersold voltage around 0.55 Volts.
- for selection the point on 1.4 vgs we will get repective Vds by doing projection on X-axis.

## NgspiceSky130 - Day 2 - Velocity saturation and basics of CMOS inverter VTC

### SPICE simulation for lower nodes and velocity saturation effect

#### L1: SPICE simulation for lower nodes

- Here we consider beyond the blue line it is linear, after the blue line it is non linear[it is a function of (1+ λ*Vds)}

<img width="400" height="252" alt="image" src="https://github.com/user-attachments/assets/2289e92f-c19d-4773-a604-bc5f7248f004" />

##### Now Spice Waveform : W= 0.375µ, L= 0.25µ device (W/L = 1.5)

- Here, by keeping W/L ratio constant

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/e12a9f2a-0001-427c-9408-8836962b96ff" />

- commands and changing the value of the W and L by using "gedit" in the day2 file in the cloud
- run the edited file by keeping W= 0.375µ, L= 0.25µ device (W/L = 1.5)
 
<img width="1113" height="727" alt="image" src="https://github.com/user-attachments/assets/33486745-b082-4ca5-9264-ba61978fe095" />

- here , the ploting of W= 0.375µ, L= 0.25µ device (W/L = 1.5) in the ngspice

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/022953ba-1dfe-4c45-9f68-77b37695d86e" />

#### L2 Drain current vs gate voltage for long and short channel device

- long channel device (> 1.20)
- short channel device (< 0.25)

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/18685893-1358-4d0d-b0e9-bb5adc057a1e" />

##### In long channel
- At saturation region, the drain current (Id) is a quadratic dependence from Vgs raised from bottom to top
- Here, at different values of Vgs at one Vds(2.5Volts) is a quadratic dependence

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/ab3233b1-350c-4016-a480-026fc55b0b11" />

- Barely look like qudratic for both lower and higher values of gate voltage(Vgs)  
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/81e493ea-4930-4a9b-b012-5cc311e9be13" />


#####  In short channel

- At saturation region, the drain current (Id) is a switching from Quadratic to Linear dependence by increasing the Vgs.
- Reason for this is Velocity Saturation in the short channels

<img width="506" height="328" alt="image" src="https://github.com/user-attachments/assets/b3ff6b1c-b3b4-40d6-af04-e655316fe734" />

Barely look like qudaratic for lower values of gate voltage and linear for higher values of gate voltage(Vgs)

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/4c6b54a7-7dc2-467d-9a4a-bf4d87937c27" />

#### L3 Velocity saturation at lower and higher electric fields

<img width="504" height="300" alt="image" src="https://github.com/user-attachments/assets/ab7bb70f-8264-413a-b991-7c64fd38a5f7" />

- Concept of Velocity Saturation Effect states that, your velocity tends to linear for lower value of electric field(ε) . after certain point (critical(εc)) velocity remains constant for higher electric field(​ε)

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/07919d03-f985-4de1-9989-1d661bff8302" />

- εc ​<= ε ----> velocity (m/sec) is linear
- εc >= ε ----> velocity (m/sec) is constant, Here we consider Saturation Velocity(Vsat)

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/bb5c19d9-f2db-4dd3-b24a-ff94759bc2a1" />

- Re-derving the drain current Equation using the boundary conditions and it become too complex.
  
<img width="504" height="308" alt="image" src="https://github.com/user-attachments/assets/2a41b2c0-16d5-449c-b49c-eafa3c1b92ef" />

##### Velocity Saturation Effect with differnt Operational Modes

- One mode of Long channel (>250nm) and another one for short channel (<250nm)
- For short channel we have velocity saturation region  more compared long channel
- Here onwards {Vgs-Vt = Vgt}

- Id = 0 , for Vgt<0 in cuttoff mode
- rest of the remaining modes we are using the following equation
- Id = (Kn)(1+ λ*Vds)[(Vgt.Vmin)- Vmin**2 / 2]  ---->  Drain Current Model
- here, Vmin = min(Vgt,Vds,Vdsat)

<img width="507" height="314" alt="image" src="https://github.com/user-attachments/assets/2c9da1e3-b861-4e99-abb8-e1f92be547bd" />

#### L4: Velocity saturation drain current model

- Vdsat ----> it is called as technology parameter
- it is a saturation voltage i.e voltage at which device velocity saturates and is independent of Vgs or Vds.
-  it is a constant value

##### When Vgt is the Minimum Value

- It comes under saturation region operation. it is true for the both the channel nodes

<img width="500" height="397" alt="image" src="https://github.com/user-attachments/assets/ad6d99a1-b170-4c4f-acab-297429fa4b75" />

##### When Vds is the Minimum Value

- it comes under resistive region operation. it is true for the both the channel nodes

<img width="500" height="393" alt="image" src="https://github.com/user-attachments/assets/39f2e4c6-d279-46c9-84b0-ae5fe4bbde37" />

##### When Vsat is the Minimum Value

- here it is **ONLY** applicable for **short channel devices**

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/56928d36-2a9f-4550-b30d-634e4f10b8c9" />

##### Observation 2

- When we move from Higher Device to Lower Device, important term to note that Velocity Saturation causes device to saturate early.
- For the same ( W/L ratio) we can observe different Peak currents

<img width="500" height="403" alt="image" src="https://github.com/user-attachments/assets/0e5dc61f-06a9-48e3-ab18-33033076c750" />

#### L5: Labs Sky130 Id-Vgs

- for running W = 0.39 and L = 0.15 (short channel)

<img width="531" height="400" alt="image" src="https://github.com/user-attachments/assets/1a09ffdb-57bf-4936-b14c-a109e2b629ca" />

##### here, is  the plot for  **IdVds**

<img width="506" height="400" alt="image" src="https://github.com/user-attachments/assets/991a7a4f-9074-4c52-ac43-c85f3e704b6a" />

- From this plot , we can observe that for lower value of Vgs we get Quadratic and higher values of the Vgs we getting linear

<img width="409" height="304" alt="image" src="https://github.com/user-attachments/assets/d7e2d15b-9126-492c-924e-6ed56b8844df" />

##### here, is  the plot for  **IdVgs**

- for running W = 0.39 and L = 0.15 (short channel)

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/f1d4fc52-2294-49b5-b052-6ceb18f78d89" />

<img width="506" height="413" alt="image" src="https://github.com/user-attachments/assets/b2bbaae7-b243-460f-9d0b-2f16bf611fe9" />

#### L6: Labs Sky130 Vt

- Lets find out theresold voltage for IdVgs curve
- To get the theresold voltage , we have to draw a tangent to the curve and mark the point where tangent is intersecting the X-axis

<img width="506" height="413" alt="image" src="https://github.com/user-attachments/assets/b2bbaae7-b243-460f-9d0b-2f16bf611fe9" />

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5eb5b6ce-4e6d-422e-ab20-2045e9692457" />

- The point of intersection of X-axis around 0.77 volts(vds).

### CMOS voltage transfer characteristics (VTC)

#### L1: MOSFET as a switch

- When ever the Vgs > Vt then only device get turn on.
- ∣Vgs∣>∣Vt​∣ then only Switch gets closed and device can do its work.
- Here, Transistor acts a Switch under the following conditions.

<img width="675" height="357" alt="image" src="https://github.com/user-attachments/assets/b40ab43b-4f28-4493-8dd7-fae904f53d97" />

- **CMOS** is Know as Complimentary MOSFET, because it can operating by using complimentary logic
- here PMOS at the top and NMOS at the bottom
- Source of PMOS connected to Vdd and Soucre NMOS connected to Vss
- Both the Gates tied together and connected to Vin
- Both of the drains tied together and connected to the Vout 
- Load(CL) could be anything, it would be loading for the next i/p transistor. it is can connected by either short or long wire.
- Vgs for NMOS is Vss-Vin (+ ve Vgs)
- Vgs for PMOS is Vin-Vdd (- ve Vgs).
- --> if Vin = 0Volts and Vdd  = Vdd Volts
- --> then Vgs = 0 - Vdd = - Vdd (full scale voltage) as the result of this PMOS will get turn on
- PMOS get turn off if Vin = Vdd and NMOS turn on































<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/e4be051b-9f05-45d1-861f-b22f36239742" />



















  












  













