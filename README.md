# CMOS Circuit Design and SPICE Simulation using SKY130 Technology Workshop

## **_Brief Description of the course_**
A structured five‑day workshop exploring CMOS fundamentals, inverter behavior, and design challenges. [VLSI System Design]( https://www.vlsisystemdesign.com/). This five‑day CMOS circuit design workshop was carefully organized to build knowledge step by step. It began with NMOS drain current (Id) and voltage transfer characteristics (VTC), then moved to velocity saturation and inverter transfer curves. The mid‑sessions focused on switching thresholds(Vt), dynamic simulations, and deriving key equations that link PMOS/NMOS sizing (W/L) ratios to the switching threshold voltage(Vm). Later, noise margins and inverter robustness were discussed, and the final day examined how variations in power supply and fabrication processes affect both single inverters and inverter chains. The workshop offered a balanced mix of theoretical derivations and practical insights into CMOS design.

## **_INDEX:_**

- [CMOS Circuit Design and SPICE Simulation using SKY130 Technology Workshop ](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#nngspicesky130---day-1---basics-of-nmos-drain-current-id-vs-drain-to-source-voltage-vds)
  
    - [Brief Description of the course](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#brief-description-of-the-course)
      
- [INDEX](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#index)

- [Day 1: Basics of NMOS Drain Current (Id) vs Drain-to-source Voltage (Vds)](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#nngspicesky130---day-1---basics-of-nmos-drain-current-id-vs-drain-to-source-voltage-vds)
  - [Part 1: Introduction to Circuit Design and SPICE simulations](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#part-1-introduction-to-circuit-design-and-spice-simulations)
  - [Part 2: NMOS Resistive region and Saturation region of operation](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#nmos-resistive-region-and-saturation-region-of-operation)
  - [Part 3: Introduction to SPICE](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#introduction-to-spice)
      - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l4-first-spice-simulation)
- [Day 2: Velocity Saturation and basics of CMOS inverter VTC](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#ngspicesky130---day-2---velocity-saturation-and-basics-of-cmos-inverter-vtc)
    - [Part 1: SPICE simulation for lower nodes and velocity saturation effect](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#spice-simulation-for-lower-nodes-and-velocity-saturation-effect)
        - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l1-spice-simulation-for-lower-nodes)
    - [Part 2: CMOS voltage transfer characteristics (VTC)](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#cmos-voltage-transfer-characteristics-vtc)
- [Day 3: CMOS switching threshold and dynamic simulations](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#ngspicesky130---day-3---cmos-switching-threshold-and-dynamic-simulations)
    - [Part 1: Voltage transfer characteristics and SPICE simulations](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#voltage-transfer-characteristics--spice-simulations)
        - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l3-labs-sky130-spice-simulation-for-cmos)
    - [Part 2: Static Behavior Evaluation - CMOS Inverter Robustness: Switching threshold](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#static-behavior-evaluation--cmos-inverter-robustness--switching-threshold)
- [Day 4: CMOS Noise Margin Robustness Evaluation](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#ngspicesky130---day-4---cmos-noise-margin-robustness-evaluation)
    - [Part 1: Static Behavior Evaluation - CMOS Inverter Robustness: Noise Margin](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#static-behavior-evaluation--cmos-inverter-robustness--noise-margin)
        
        - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l5-sky130-noise-margin-labs)
- [Day 5: CMOS Power supply and device variation robustness evaluation](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#ngspicesky130---day-5---cmos-power-supply-and-device-variation-robustness-evaluation)
    - [Part 1: Static Behavior Evaluation - CMOS Inverter Robustness: Power Supply Variation](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#static-behavior-evaluation--cmos-inverter-robustness--power-supply-variation)
        
        - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l3-sky130-supply-variation-labs)
    - [Part 2: Static Behavior Evaluation - CMOS Inverter Robustness: Device Variation](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#static-behavior-evaluation--cmos-inverter-robustness--device-variation)
        
        - [Lab Activity](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#l5-sky130-device-variation-labs)
- [Conclusion and Opinion](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#conclusion-and-opinion)
- [References](https://github.com/Dinesh30P/Cmos_Circuit_design_SPICE_SIMULATION/tree/main?tab=readme-ov-file#references)


# NNgspiceSky130 - Day 1 : Basics of NMOS Drain current (Id) vs Drain-to-source Voltage (Vds)

## Part-1: Introduction to Circuit Design and SPICE Simulations 

## CMOS_Circuit_Design_&_SPICE_SIMULATION
 
### L1: Why is SPICE Simulation Needed?
- To verify circuit behavior before fabrication.
-  To optimize the Performance.
-  To reduce the Cost and improve timing efficiency.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/d0cd4084-6e16-4550-97e7-6f5c899e44ce" />


##### What is circuit design and SPICE?
- circuit design consists of logic gates AND,OR,NOT,Buffer...made up of PMOS and NMOS transistors connected in particular fasion.
- SPICE is a Simulation Program with Integrated Circuit Emphasis, which genereats the waveform defines the delay of the pariticlar cell based on the waveform shape.

##### Why do we need SPICE?
- The clocktree synthesis, timing, crosstalks are build on the SPICE, without having SPICE there won't be delays and if there is no delays physical design flow, crosstalk won't make any sense.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/ea9a8b75-a1f8-4b46-9179-3cd58b61fc3f" />

##### Clocktree sysnthesis
- delay table consists of  i/p slew and o/p load for buffer types (level 1, level 2)
- intersection value consider as the delay
- if the delay table not provide any value then we have to do interpolation between two values through equations
- Each transistor (PMOS & NMOS) is unique, with different delay values and buffer sizing (W & L) delay behavior and determines current.
- Buffer differentiation is part of circuit design.
- Length(L) and  Width(W)  decide the Drive current (I) that results in the timing curves.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/caded01a-8ef3-44c6-adc9-2f13e7e38b9a" />

### L2: Introduction to basic element in Circuit design – NMOS

A transistor is a semiconductor device that can control the current flow through an electric field and functions mainly as an amplifier or a switch. The MOS transistor is the core device mostly used in CMOS circuits. A MOS transistor can be either n-type (NMOS) or p-type (PMOS) depending on the doping and dominant charge carriers.

|Component          | Description        |     Key Notes                    |
|---------------------------|--------------------|--------------------------------------------------------|
|P‑type Substrate      | Base semiconductor foundation                   | - Serves as the body  <br> - Provides holes as majority carriers |
| Isolation Region | Areas separating nearby devices | - Prevents electrical interaction <br> - Reduces leakage and latch‑up risks |
| Gate Oxide | Thin insulating layer above substrate | - Commonly SiO₂ <br> - Governs channel creation <br> - Influences threshold voltage |
| Polysilicon / Metal Gate | Conductive layer placed over gate oxide| - Acts as the Gate terminal <br> - Controls channel via electric field <br> -Enables switching |
| Body Terminal | Substrate connection point | - Often grounded in NMOS <br> - Impacts threshold voltage (body effect) <br> - Important for modeling |

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/ee5ea8b2-ae84-4e63-8b09-3ab224b7b79d" />

#### Threshold Voltage:
- Threhold Voltage (Vt) is the gate voltage,when grounded all termimals, starting from zero, and gradully increasing postively, until it reaches minimum volatage required to form a conductive channel between the source and drain to turn on the NMOS.
- It is a function of x,y,z. which can accurately describes the NMOS Transistor. Here we called as Models.
#### Modeling of Threshold Volatage

- Let, consider Vgs=0
- Source, Connect Drain, and Body to GND
- Now, Source-Body and Drain-Body acts as a pn junction diode
- As both junctions are OFF, there is a huge resistance between Source and Drain, thus no conductivity between Source and Drain.
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/20b7652d-1b59-42d7-bfcc-6b73ef21a153" /> <br>

- When a small positive voltage is applied to the gate, an electric field is established across the gate oxide.
- Then the gate oxide acts as a capacitor, causing repells the holes(postive charges) in the p-type substrate deeper into the substrate, leaving behind immobile negative ions near the surface.
- As the negative charges are accumulate near to the gate oxided, a depletion region forms (depleting the majority charge carries) inside the NMOS near to the surface.
   
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/814aeeb1-24a2-4507-81fb-25d131c3f4ae" />

### L3: Strong inversion and threshold voltage

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

### L4: Threshold voltage with positive substrate potential

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

## Part-2: NMOS resistive region and saturation region of operation

### L1: Resistive region of operation with small drain-source voltage

#### Resistive Operation
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

### L2: Drift current theory
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

### L3: Drain current model for linear region of operation

- velocity is Vn(x), W is width, mobility of the carriers and electric field

<img width="400" height="310" alt="image" src="https://github.com/user-attachments/assets/a85ac293-afbd-4ead-aa22-1382629a3d76" />

- Substituing and Intergrating dx over channel lenght L will give the V-I relation of NMOS transistor.

<img width="405" height="307" alt="image" src="https://github.com/user-attachments/assets/e0ff3e90-7c15-44f2-88f7-36576ca0c9b6" />

- when ever (Vds <= Vgs-Vt) MOSFET operates in the linear region.

#### Current Equation for Linear Region 

Id = (Kn)*{(Vgs-Vt)Vds - Vds**2 / 2} 
  
<img width="503" height="406" alt="image" src="https://github.com/user-attachments/assets/b955d07a-bbea-4164-a6ef-946645add5c3" />

### L4: SPICE conclusion to resistive operation

- For linear region operation we have to make sure that  (Vds <= Vgs-Vt) so we neglection the 
Vds^2 / 2 term in the current equation.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/31b06dbb-93c9-46de-a840-4eb047d1a460" />

- here we have sweep the values of Vds ranging for 0 to 2.05 but maintaining the condition         Vds <= Vgs-Vt to be in the linear region or restitve region of operation.
- if Vds >= Vgs-Vt then device enters into the saturation region

### L5 Pinch-off region condition

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
#### Pinch of Phenomenon Started
- i.e channel begins to disappear(linearity of the current flow changes)
- At this point Vt = Vgs-Vds(surface iversion just happens / about to happen )

<img width="504" height="402" alt="image" src="https://github.com/user-attachments/assets/d197b2b5-2be4-44da-958c-e235c6dcfd13" />

#### Pinch off Region

-  here Vgs-Vds < Vt(no channel present near to the drain)
 
-  <img width="500" height="444" alt="image" src="https://github.com/user-attachments/assets/685c7cf4-2b31-4383-87a7-d2d95e2d91cd" />

### L6: Drain current model for saturation region of operation

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

#### Constant Current Equation for Saturation Region 

- Id = (Kn'/2)(W/L)(1+ λ*Vds)(Vgs-Vt)**2

## Part-3:Introduction to SPICE

### L1 Basic SPICE setup

- It is basically a software and its an engine which can derives some waveform by giving inputs
- This waveforms are used to calculate the delay of the cell
- This delays are accurate and used to Static Timing Analysis(STA)

#### SPICE Model Parameters 

- The highlighted ones are the constants will come from the foundaries when we tackle advance technology nodes

<img width="512" height="321" alt="image" src="https://github.com/user-attachments/assets/eb44d327-72f0-4f90-8070-435ce1113d0e" />

#### SPICE setup Flow chart

<img width="506" height="401" alt="image" src="https://github.com/user-attachments/assets/b60bbe86-2c9a-4c0b-9ed6-22a0167b0837" />

##### Spice Netlist 

- A SPICE netlist is a plain text file that defines the components and connections of an electronic circuit, allowing it to be analyzed and simulated using SPICE software.

<img width="503" height="396" alt="image" src="https://github.com/user-attachments/assets/088e3d30-d3eb-455e-9a0b-fa1683dce2c4" />

### L2: Circuit description in SPICE syntax

- let's give the values for the netlist
- Here, We can considering 4 nodes (where there is no obstraction we can consider as node)

<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/3998d2e2-e461-4278-9b9f-3169d6be1a5a" />

- In an electrical circuit, a node is a point where two or more components are connected together. It represents a location where the electrical potential (voltage) is the same for all connected elements.
- Nodes are used in circuit analysis to determine voltages and currents throughout the system.

#### DGSS
  
<img width="506" height="409" alt="image" src="https://github.com/user-attachments/assets/7da08862-1bc6-4461-a3c7-9d434fcc8125" />

- MOSFET have 4 terminals i.e Drain, Gate, Source, Substrate/Bulk
- 
#### For the First Component (MOSFET)
- M1 --> MOSFETXX (XX- number), Vdd --> Drain, 0 --> Source node, 0 --> Substrate node, NMOS --> it comes from technology file, W= 1.8µ --> Width of the Gate in microns, L = 1.2µ --> length of the Gate in Micron.

#### For the Second Componet (Resistor)
- R1 --> ResistorXX (XX- number), in --> First terminal, n1 --> Node 1 {R1 is between in and n1}, 55 Ω --> Resistance  Value in Ohms

#### Vdd Source 

- VXX --> Voltage source XX(it will between 2 nodes i.e Vdd and Zero), here  Vdd is 2.5 Volts.
- Vin lies in between in(postive terminal)and Zero (negative terminal), here  Vin is 2.5 Volts.
- Once we define the netlist, next we have to define the technology file.

<img width="420" height="200" alt="image" src="https://github.com/user-attachments/assets/4bd4c5c2-375c-48c6-8573-4312ff961239" />


### L3: Define Technology Parameters
 
#### Models
 - AND gate is a BOOLEAN Multiplication of two inputs
 - OR gate is a BOOLEAN Addition of two inputs

#### For Model Files(Vt,Id...) --> Model Parameters(γ, kn'/2...) are Required

<img width="539" height="404" alt="image" src="https://github.com/user-attachments/assets/163ce3ae-2771-45a8-bcf2-1ffe17f7e2b2" />

- for Nmos model file we have to choose NMOS package (its very important)

<img width="501" height="403" alt="image" src="https://github.com/user-attachments/assets/8cacb959-fbbd-408b-8e41-cfbc1df79ad0" />

#### Package in a file (.mod )

#### .LIB "xxxx_025µm_model.mod" CMOS_MODELS

#### Simulation commands
- We have to Sweep Drain and Gate Voltage

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/4f64cabc-50ae-41a2-b857-92f23dda6bfc" />

### L4: First SPICE simulation

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

# NgspiceSky130 - Day 2 : Velocity saturation and basics of CMOS inverter VTC

## Part-1: SPICE simulation for lower nodes and velocity saturation effect

### L1: SPICE simulation for lower nodes

- Here we consider beyond the blue line it is linear, after the blue line it is non linear[it is a function of (1+ λ*Vds)}

<img width="400" height="252" alt="image" src="https://github.com/user-attachments/assets/2289e92f-c19d-4773-a604-bc5f7248f004" />

#### Now Spice Waveform : W= 0.375µ, L= 0.25µ device (W/L = 1.5)

- Here, by keeping W/L ratio constant

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/e12a9f2a-0001-427c-9408-8836962b96ff" />

- commands and changing the value of the W and L by using "gedit" in the day2 file in the cloud
- run the edited file by keeping W= 0.375µ, L= 0.25µ device (W/L = 1.5)
 
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/33486745-b082-4ca5-9264-ba61978fe095" />

- here , the ploting of W= 0.375µ, L= 0.25µ device (W/L = 1.5) in the ngspice

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/022953ba-1dfe-4c45-9f68-77b37695d86e" />

### L2 Drain current vs gate voltage for long and short channel device

- long channel device (> 1.20)
- short channel device (< 0.25)

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/18685893-1358-4d0d-b0e9-bb5adc057a1e" />

#### In long channel
- At saturation region, the drain current (Id) is a quadratic dependence from Vgs raised from bottom to top
- Here, at different values of Vgs at one Vds(2.5Volts) is a quadratic dependence

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/ab3233b1-350c-4016-a480-026fc55b0b11" />

- Barely look like qudratic for both lower and higher values of gate voltage(Vgs)  
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/81e493ea-4930-4a9b-b012-5cc311e9be13" />


####  In short channel

- At saturation region, the drain current (Id) is a switching from Quadratic to Linear dependence by increasing the Vgs.
- Reason for this is Velocity Saturation in the short channels

<img width="506" height="328" alt="image" src="https://github.com/user-attachments/assets/b3ff6b1c-b3b4-40d6-af04-e655316fe734" />

Barely look like qudaratic for lower values of gate voltage and linear for higher values of gate voltage(Vgs)

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/4c6b54a7-7dc2-467d-9a4a-bf4d87937c27" />

### L3 Velocity saturation at lower and higher electric fields

<img width="504" height="300" alt="image" src="https://github.com/user-attachments/assets/ab7bb70f-8264-413a-b991-7c64fd38a5f7" />

- Concept of Velocity Saturation Effect states that, your velocity tends to linear for lower value of electric field(ε) . after certain point (critical(εc)) velocity remains constant for higher electric field(​ε)

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/07919d03-f985-4de1-9989-1d661bff8302" />

- εc ​<= ε ----> velocity (m/sec) is linear
- εc >= ε ----> velocity (m/sec) is constant, Here we consider Saturation Velocity(Vsat)

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/bb5c19d9-f2db-4dd3-b24a-ff94759bc2a1" />

- Re-derving the drain current Equation using the boundary conditions and it become too complex.
  
<img width="504" height="308" alt="image" src="https://github.com/user-attachments/assets/2a41b2c0-16d5-449c-b49c-eafa3c1b92ef" />

#### Velocity Saturation Effect with differnt Operational Modes

- One mode of Long channel (>250nm) and another one for short channel (<250nm)
- For short channel we have velocity saturation region  more compared long channel
- Here onwards {Vgs-Vt = Vgt}

- Id = 0 , for Vgt<0 in cuttoff mode
- rest of the remaining modes we are using the following equation
- Id = (Kn)(1+ λ*Vds)[(Vgt.Vmin)- Vmin**2 / 2]  ---->  Drain Current Model
- here, Vmin = min(Vgt,Vds,Vdsat)

<img width="507" height="314" alt="image" src="https://github.com/user-attachments/assets/2c9da1e3-b861-4e99-abb8-e1f92be547bd" />

### L4: Velocity saturation drain current model

- Vdsat ----> it is called as technology parameter
- it is a saturation voltage i.e voltage at which device velocity saturates and is independent of Vgs or Vds.
-  it is a constant value

#### When Vgt is the Minimum Value

- It comes under saturation region operation. it is true for the both the channel nodes

<img width="500" height="397" alt="image" src="https://github.com/user-attachments/assets/ad6d99a1-b170-4c4f-acab-297429fa4b75" />

##### When Vds is the Minimum Value

- it comes under resistive region operation. it is true for the both the channel nodes

<img width="500" height="393" alt="image" src="https://github.com/user-attachments/assets/39f2e4c6-d279-46c9-84b0-ae5fe4bbde37" />

#### When Vsat is the Minimum Value

- here it is **ONLY** applicable for **short channel devices**

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/56928d36-2a9f-4550-b30d-634e4f10b8c9" />

#### Observation-2

- When we move from Higher Device to Lower Device, important term to note that Velocity Saturation causes device to saturate early.
- For the same ( W/L ratio) we can observe different Peak currents

<img width="500" height="403" alt="image" src="https://github.com/user-attachments/assets/0e5dc61f-06a9-48e3-ab18-33033076c750" />

### L5: Labs Sky130 Id-Vgs

- for running W = 0.39 and L = 0.15 (short channel)

<img width="531" height="400" alt="image" src="https://github.com/user-attachments/assets/1a09ffdb-57bf-4936-b14c-a109e2b629ca" />

#### here, is  the plot for  **IdVds**

<img width="506" height="400" alt="image" src="https://github.com/user-attachments/assets/991a7a4f-9074-4c52-ac43-c85f3e704b6a" />

- From this plot , we can observe that for lower value of Vgs we get Quadratic and higher values of the Vgs we getting linear

<img width="409" height="304" alt="image" src="https://github.com/user-attachments/assets/d7e2d15b-9126-492c-924e-6ed56b8844df" />

#### here, is  the plot for  **IdVgs**

- for running W = 0.39 and L = 0.15 (short channel)

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/f1d4fc52-2294-49b5-b052-6ceb18f78d89" />

<img width="506" height="413" alt="image" src="https://github.com/user-attachments/assets/b2bbaae7-b243-460f-9d0b-2f16bf611fe9" />

### L6: Labs Sky130 Vt

- Lets find out theresold voltage for IdVgs curve
- To get the theresold voltage , we have to draw a tangent to the curve and mark the point where tangent is intersecting the X-axis

<img width="506" height="413" alt="image" src="https://github.com/user-attachments/assets/b2bbaae7-b243-460f-9d0b-2f16bf611fe9" />

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5eb5b6ce-4e6d-422e-ab20-2045e9692457" />

- The point of intersection of X-axis around 0.77 volts(vds).

## Part-2: CMOS voltage transfer characteristics (VTC)

### L1: MOSFET as a switch

- When ever the Vgs > Vt then only device get turn on.
- ∣Vgs∣>∣Vt​∣ then only Switch gets closed and device can do its work.
- Here, Transistor acts a Switch under the following conditions.

<img width="500" height="407" alt="image" src="https://github.com/user-attachments/assets/b40ab43b-4f28-4493-8dd7-fae904f53d97" />

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

<img width="500" height="403" alt="image" src="https://github.com/user-attachments/assets/66f2a542-383b-4e0c-8ede-c5868f137e02" />

### L2: Introduction to standard MOS voltage current parameters

- To turn on PMOS -Vgs is less than -Vt
- Vin is Low and equal to "0 V"

<img width="500" height="402" alt="image" src="https://github.com/user-attachments/assets/c430e8f6-94f0-454c-8a26-3bc99faddf50" />

#### We are watching the voltage conditions

- It is very important to know the direction of current
- all the CL got discharge then Vout is zero, due direct path exist between Vout and Vss

<img width="504" height="309" alt="image" src="https://github.com/user-attachments/assets/3bce9881-5952-4faa-961d-42176c7efe42" />

- Direction of the current flow is important
- we adding more  meaningful conventions 

<img width="501" height="402" alt="image" src="https://github.com/user-attachments/assets/25651aa5-a1ef-4fe9-8ac4-ce99e51f9087" />


### L3 PMOS/NMOS drain current v/s drain voltage

##### By Observation

<img width="507" height="379" alt="image" src="https://github.com/user-attachments/assets/6172ff7c-10a9-4a49-8de4-9c1c64a2a2b8" />

- VgsN = Vin - Vss = **Vin**
- VdsN = **Vout**
- VgsP =  **Vin - Vdd** (carefully rememeber not only Vin and also less than thersold voltage to get turn on)
- VdsP =  **Vout - Vdd**
- IdsP = (-) IdsN

#### Derving the load current

- NMOS IdsN vs VdsN Curve
- PMOS IdsP vs VdsP Curve (is Inversion of the NMOS)
  
<img width="502" height="309" alt="image" src="https://github.com/user-attachments/assets/d0cf7e41-1dfa-44ae-83ec-0d96536f10bd" />

### L4: Step1 – Convert PMOS gate-source-voltage to Vin

- When ever input Voltage goes from 0 to 1.
- The output voltage will goes from logic 1 to logic 0 on the application of 0 to 1.
- All of them are in the function of Vin and Vout only.
- The internal node voltages are not even visible to a user, because those are not use in any kind of digital device

#### Voltage tranfer characterstics

<img width="500" height="404" alt="image" src="https://github.com/user-attachments/assets/447c669a-e5f0-40e2-9e61-77e2d4834563" />

- Shifting of the curve takes place IdsP to IdsN
- By using this formula
   --> Vin - Vdd = VgsP
   --> Vin = VgsP + Vdd
- Here Vdd = 2 volts
- Converting all Vgsp into Vin


### L5 Step2 & Step3: – Convert PMOS and NMOS drain-source-voltage to vout

- Mirror Image with respective X-axis(IdsP = -IdsN)
- we have to convert the whole curve into Vout
- Vout = 0 ,there is a finite current flow, then the capacitance of the ouput capacitor is completely discharge . We need to charge the capacitance.
- This comes when PMOS is clud together with NMOS (not independent one)

 --> VdsP = Vout - Vdd
 --> Vout = VdsP + Vdd (Vdd = 2V)

- By shifting the curve with the Value of Postive Vdd
- after shifting by Vdd then  Vout = 2V then current is to be zero, its states that output capcitor is completely charge.
- Load curve for PMOS which is a function of Vin an Vout

<img width="500" height="304" alt="image" src="https://github.com/user-attachments/assets/aebfe707-27b4-445c-8a4c-a31a346a549f" />

#### Load Curve for NMOS transistor using the above equations

- just changing the Nable by using this equations and plot the values as same Id vs VdsN
- VgsN = Vin - Vss = Vin
- VdsN = Vout

<img width="507" height="396" alt="image" src="https://github.com/user-attachments/assets/46190be0-d906-4747-8e2a-7e1a4dbc1e82" />

<img width="408" height="319" alt="image" src="https://github.com/user-attachments/assets/4f806b17-62a2-4f7f-8d38-d249d5735f63" />

- By merging the two curves in the Vin and Vout

<img width="505" height="304" alt="image" src="https://github.com/user-attachments/assets/c126f794-1f01-460d-aa91-bf0dcc43a9b8" />

#### L6: Step4 – Merge PMOS – NMOS load curves and plot VTC

- By superimposing 2 curves and identify the intersection points where PMOS and NMOS meets according to the operation modes (Vout Vs Vin)
- When from the PMOS curve, Vin = 0 and Vout = 2. Here, NMOS is in Cutoff region i.e completely turned off and PMOS is in Linear region.
- When from the PMOS curve, Vin = 0.5 and 1.5 < Vout < 2. Here, NMOS is in Saturation region  and PMOS is in Linear region.
- When from the PMOS curve, Vin = 1 and 0.5 < Vout < 1.5. Here, NMOS is in Saturation region and PMOS is in Saturation region.
- Here is the area for the CMOS for high Gain state. any little change in the input huge impact in the output. preferable for most of the anlog devices.
- When from the PMOS curve, Vin = 1.5 and 0 < Vout < 0.5. Here, NMOS is in Linear region and PMOS is in Saturation region.
- When from the PMOS curve, Vin = 2 and Vout = 0. Here, NMOS is in cutoff region i.e completely turned off and PMOS is in Saturation region.

<img width="503" height="401" alt="image" src="https://github.com/user-attachments/assets/d751ba5b-ddc5-4a0a-b023-3b182ad674f2" />

# NgspiceSky130 - Day 3 : CMOS Switching threshold and dynamic simulations
## Part-1: Voltage transfer characteristics – SPICE simulations

### L1: SPICE deck creation for CMOS inverter

####  VTC Spice Simulations

- Spice deck is a connectivity information about the netlist
- It has Connectivity Information, it also provide input to the simulation, it also having tap points at which we can take the output
- Here, we are making spice deck for complete netlist
- We also looking into significance of Substrate pin, where it tunes thersold voltage of PMOS and NMOS.
- ideally PMOS is twice or thrice than NMOS component values i.e (W/L) .
- but here considering same componets for both PMOS and NMOS.
- Usually voltage(2.5 V) kept multiple of channel length(0.25 x 10)
- Identify the nodes
- Node : there is a component between two points.
- Node names : in , out, Vdd, 0

<img width="505" height="390" alt="image" src="https://github.com/user-attachments/assets/91e2aede-9a68-4f5e-80b8-fa3a062ae9d6" />

### L2: SPICE simulation for CMOS inverter

<img width="560" height="412" alt="image" src="https://github.com/user-attachments/assets/3fd0246b-ba45-4c97-846a-79eb50a6958e" />

- Spice Waveform : Wn = Wp = 0.375µ, Ln,p = 0.25µ device (Wn/Ln = Wp/Lp= 1.5)
- Edit the file by the Required parameters

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/b4f6b417-cb4a-4afd-927c-3ba315dc3f57" />

### L3 Labs Sky130 SPICE simulation for CMOS

-  Spice Waveform : Wn = 0.36µ, Wp = 0.84µ, Ln,p = 0.15µ device (Wn/Ln = 2.4, Wp/Lp= 5.6)
- By using Vim command check the file which already existing in the folder.
- By using ":q" to quit without changing the file.
- Run the ngspice and file name 
- Now using plot command "**plot out vs in**"

- This is the required plot
  
<img width="500" height="402" alt="image" src="https://github.com/user-attachments/assets/3fc14f8a-d767-49bc-8a01-0db92cff4180" />

- This is the dervied plot
  
<img width="502" height="409" alt="image" src="https://github.com/user-attachments/assets/b0e80393-b728-4f96-a268-5da6a27e95a1" />

### Now doing transient analysis

- By using Vim command check the file which already existing in the folder.
- By using ":q" to quit without changing the file.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/7d421fa7-b889-4670-aedf-fc8f724b28e7" />

<img width="503" height="404" alt="image" src="https://github.com/user-attachments/assets/843b1e31-49c6-4d80-8b64-d937fa78d08c" />

<img width="606" height="450" alt="image" src="https://github.com/user-attachments/assets/a264e1a0-71a5-4be0-a9ad-a691256d2e12" />

- For rise delay and Fall delay we have to consider 50% of Vdd
- Here, 1.8/2 is 0.9 (vdd)

#### For Rise Delay

- Zoom out the area out curve (red)- in curve(blue)

<img width="503" height="404" alt="image" src="https://github.com/user-attachments/assets/1eb0a52c-6ede-4c7d-89cc-9da9f5195d04" />

- At point 0.9, **Xout - Xin**

<img width="400" height="302" alt="image" src="https://github.com/user-attachments/assets/6087a627-fb46-496c-96c7-00f6791e8bdb" />

- Rise Delay {Xout - Xin} = (2.482- 2.151)e-9 = 0.331e-9 secs =0.331 ns.

#### For Fall Delay

- Zoom out the area out curve (red)- in curve(blue)

<img width="500" height="402" alt="image" src="https://github.com/user-attachments/assets/6c0496da-e4df-4bcb-af35-4b22599bd728" />

- At point 0.9, **Xout - Xin**

<img width="383" height="101" alt="image" src="https://github.com/user-attachments/assets/a2e4aafe-581a-4754-9aa4-0913a3026aac" />

- Fall Delay {Xout - Xin} = (4.333 - 4.05)e-9 = 0.2818e-9 =0.2818

## Part-2: Static behavior evaluation – CMOS inverter robustness – Switching Threshold
### L1: Switching Threshold, Vm

- Spice Waveform : Wn = Wp = 0.375µ, Ln,p = 0.25µ device (Wn/Ln = Wp/Lp= 1.5)
-  Spice Waveform : Wn = 0.375µ, Wp = 0.9375µ, Ln,p = 0.25µ device (Wn/Ln = 1.5, Wp/Lp= 3.75)
- By ploting them, shape of the waveform almost same it implies that CMOS inverter is a Robust device.
- For Robust design of CMOS logic is widely used for any of the logic gate design

<img width="516" height="406" alt="image" src="https://github.com/user-attachments/assets/5ecce938-1ccc-416a-a6dd-df135886d605" />

- **Switching Thresold (Vm)** is a point whre Vin is Equal to Vout
- By Drawing a line having slope of 45 degress with X-axis and Identify a Point which is intersecting the point on the curve
- This are where both PMOS and NMOS are in the Saturation Region
- If both are turn on there is high chances of leakage current (high possibility the current flow from directly power to ground )
- When Vin = Vout then gate Voltage is Equal to Drain Voltage i.e Vgs is >>> Vt
- When Vgs = Vds , the Current flow in the Output side is almost same but direction are different.(IdsP = (-) IdsN)

<img width="502" height="402" alt="image" src="https://github.com/user-attachments/assets/c6a9a803-b9fe-4f6a-9160-79b837389914" />

### L2: Analytical expression of Vm as a function of (W/L)p and (W/L)n

- IdsP + IdsN = 0

<img width="530" height="405" alt="image" src="https://github.com/user-attachments/assets/9278d903-681c-450d-96c3-0fe4183063f5" />

- Caluclating IdsN and IdsP

<img width="509" height="403" alt="image" src="https://github.com/user-attachments/assets/413509ff-0ef9-4b43-a2e6-03de707fcaec" />

- Here R is the Constant

<img width="569" height="400" alt="image" src="https://github.com/user-attachments/assets/93c7496a-5719-44bd-a9ad-d91aa9e4dca3" />

### L3: Analytical expression of (W/L)p and (W/L)n as a function of Vm

- We derving the conditions, Exactly half of the power supply voltage. To achive that what should be the value of W/L ratio of PMOS and NMOS.
- Alternatively , the required ratio of PMOS v/s NMOS transistor size can be derived, such that Vm is Set

<img width="407" height="300" alt="image" src="https://github.com/user-attachments/assets/3f7158a8-cfd3-4161-8fa0-abdc6ad9a22b" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/9ab5f294-13e1-40fb-8fc9-6a7787709b4a" />

- Here we are getting the relation into the Vm

<img width="408" height="300" alt="image" src="https://github.com/user-attachments/assets/50d7543f-1ab5-4a9a-8e15-6e343b08e9b5" />

- By simply the equation we are able to get the following relation
  
<img width="408" height="300" alt="image" src="https://github.com/user-attachments/assets/6d56bb9d-65be-431d-a113-8e1e0b0b0802" />

- Here , We getting the value of (W/L) PMOS  = x * (W/L) NMOS

### L4: Static and dynamic simulation of CMOS inverter

- By using this relation we able to do some SPICE simulations

<img width="244" height="203" alt="image" src="https://github.com/user-attachments/assets/c22c0d27-389a-4c0e-880f-f0d46ec008a6" />

<img width="507" height="400" alt="image" src="https://github.com/user-attachments/assets/117269b5-4d10-48d3-ab1a-2584e326bd7c" />

### L5 Static and dynamic simulation of CMOS inverter with increased PMOS width

- Here the  static and dynamic simulation with Increased PMOS

<img width="518" height="406" alt="image" src="https://github.com/user-attachments/assets/b44874f4-485b-45b7-b5e4-31392bf5ae0d" />

- Rougly we able to get the Vm value (1.25V), to increase the Size of the PMOS  then curve shift towards the right side

<img width="504" height="407" alt="image" src="https://github.com/user-attachments/assets/43e8ecbc-8da5-499f-8953-1deaa833f926" />

- Rougly we able to get the Vm value (1.35V), to increase the Size of the PMOS  then curve shift towards the right side

<img width="503" height="402" alt="image" src="https://github.com/user-attachments/assets/391fd05e-db04-4390-9d93-bf40c7474308" />

- Rougly we able to get the Vm value (1.4V), to increase the Size of the PMOS  then curve shift towards the right side

<img width="500" height="404" alt="image" src="https://github.com/user-attachments/assets/31c3659b-bb54-4994-bd95-4bc51b0ee904" />

- Rise delay significantly reduses (the time required to charge the output capacitor completely)
- While increasing the size of the PMOS then rise delay decreases significantly(bigger area is the reason)

<img width="530" height="309" alt="image" src="https://github.com/user-attachments/assets/fd4097f5-f986-478e-8693-9d62684292f9" />

### L6: Applications of CMOS inverter in clock network and STA

- There is 50mv change by varing the PMOS and (multiple of  two to three )NMOS parameter


<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/1352945e-cdf5-4bdb-afa7-6d49b5116ebe" />

- There is Equal rise and fall time at vm = 1.2V
- Approximately equal rise-fall delay Typical characterstic for a clock inverter / Buffer
- Even PMOS is bigger than the NMOS the resistance of them are almost same

<img width="309" height="412" alt="image" src="https://github.com/user-attachments/assets/69fecf44-bf30-4571-ae36-478a3c3cfcb9" />

#### Irregular Inverter / Buffer

<img width="416" height="305" alt="image" src="https://github.com/user-attachments/assets/1cd15c56-2519-4bc3-84ed-eb337f4276ec" />

- The condtion for here is either Slack should be Positive or Zero
- Data arrival time < Data required time

<img width="508" height="405" alt="image" src="https://github.com/user-attachments/assets/5d94de2b-5b73-4b1c-b40a-ed33e4ad0ca3" />

- For Clock tower we are using Inv_cx and rest of them called as Inv_1x,Inv_2x,Inv_3x,Inv_4x

- One can used as Clock cell and rest of them can used as data path

# NgspiceSky130 - Day 4 - CMOS Noise Margin robustness evaluation
## Part-1: Static behavior evaluation – CMOS inverter robustness – Noise margin

### L1: Introduction to noise margin

- Consider basic Inverter when i/p is 0 then o/p is 1 and vise verse

- Noise Margin: Noise margin is the amount of unwanted disturbance (noise voltage) that a digital circuit can tolerate without changing its intended logic state.

- Vil = input Low Voltage
- Vih = input High Voltage
- Vol = output Low Voltage
- Voh = output High Voltage

- High Noise Margin(HNM) = Voh - Vih (high)
- Low Noise Margin(LNM) = Vil- Vol (low)

<img width="500" height="412" alt="image" src="https://github.com/user-attachments/assets/5b026032-2883-48fa-8f48-1f19136941d8" />

### L2: Noise margin voltage parameters

- Slope is the change in the output voltage /  change in the input voltage
- Here slope is negative

<img width="500" height="402" alt="image" src="https://github.com/user-attachments/assets/1fd29308-36e7-4efd-b3cf-2177fab31c8e" />

- Acutal one on the left side and ideal one on the right side

### L3: Noise margin equation and summary
- Here Voh > Vih(always)
- Next stage detect as logic 1
- Here Vol < Vil
- Next stage detect as logic 0

<img width="505" height="400" alt="image" src="https://github.com/user-attachments/assets/02403974-36f6-441b-aa65-e9ed2a32ac98" />

- High Noise Margin(HNM) = Voh - Vih (high)
- Low Noise Margin(LNM) = Vil- Vol (low)

- Noise induced bump chracterstics at different noise margin levels

<img width="506" height="360" alt="image" src="https://github.com/user-attachments/assets/ef9f94ad-66e8-425e-a6b3-4106e4403fd8" />

- First case, Bump height lies between Vol and Vil will be considered as Logic '0'. (safe glitch)
- Second case, Bump height lies between Vil and Vih . o/p logic "undefine".(unsafe glitch)
- Third case, Bump height lies between Vih and Voh . Will be considered as Logic'1' (safe glitch)

### L4: Noise margin variation with respect to PMOS width

- By keeping value (x) = 1 and getting the logic 0 and logic 1 by doing porjection of curve on Y-axis
- Here Vm = 0.99 V

<img width="500" height="407" alt="image" src="https://github.com/user-attachments/assets/415116a8-bb35-4479-9ab9-ec371b8104f4" />

- By keeping value (x) = 2 and getting the logic 0 and logic 1 by doing porjection of curve on Y-axis
- Here Vm = 1.2 V

<img width="502" height="401" alt="image" src="https://github.com/user-attachments/assets/1d170764-8f8c-4cff-86c5-71e8a24e3df3" />

- By keeping value (x) = 3 and getting the logic 0 and logic 1 by doing porjection of curve on Y-axis
- Here Vm = 1.25 V

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/68b32742-c4f4-4558-a6de-508f2ed08bfd" />

- By keeping value (x) = 4 and getting the logic 0 and logic 1 by doing porjection of curve on Y-axis
- Here Vm = 1.35 V

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/16531dba-ef22-4ec6-9efb-5a893defa86f" />

- By keeping value (x) = 5 and getting the logic 0 and logic 1 by doing porjection of curve on Y-axis
- Here Vm = 1.4 V

<img width="518" height="409" alt="image" src="https://github.com/user-attachments/assets/3434eb07-6e83-4b7d-8243-0400f801cb1d" />

- Here the table is plotted based on the obtain values of NMH and NML

<img width="502" height="400" alt="image" src="https://github.com/user-attachments/assets/e9c6c56e-8e4a-4804-8314-1b03bb66ff79" />

- From the above Values we can conclude that logic 0 and logic 1 area are favoarable in the digital design
- Undefined region favorable for the analog design

<img width="500" height="410" alt="image" src="https://github.com/user-attachments/assets/a2f16574-fc5a-4b4d-a32a-e7bcb9e6502b" />

### L5: Sky130 Noise margin labs

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/dcb1ccef-18bc-48a4-b9b8-fb72bd6d0f35" />

<img width="500" height="403" alt="image" src="https://github.com/user-attachments/assets/2e7ff912-9278-4a9e-9507-6dc39e7715be" />

<img width="508" height="407" alt="image" src="https://github.com/user-attachments/assets/7e6dd41c-2aee-45a7-9a83-cdbdcba042c5" />

- Here X value is ViL and Y value is VoH (slope at the top bend)

  - ViL = 0.758 and VoH = 1.722

- Here X Value is ViH and Y value is VoL(slope at the bottom bend)

 - ViH = 0.975 and VoL = 0.113

 - High Noise Margin(HNM) = Voh - Vih = 1.722 - 0.975 = 0.747
 - Low Noise Margin(LNM) = Vil- Vol = 0.758 - 0.113 = 0.645

# NgspiceSky130 - Day 5 : CMOS power supply and device variation robustness evaluation
## Part-1: Static Behavior Evaluation – CMOS inverter robustness – Power supply variation

### L1: Smart SPICE simulation for power supply variations

- We are analysing static behavior EValuation :CMS inverter Robudstness
- By keeping (W/L) ratio of PMOS to NMOS cosntant and sweeping the Vdd from 2.5 V to 1 V

<img width="516" height="400" alt="image" src="https://github.com/user-attachments/assets/5fec8a4d-dc7c-4f5a-98bc-228368dcfada" />

- Anything that comes between .control and .endc we can able to do scripting (variables , loops...)

<img width="509" height="408" alt="image" src="https://github.com/user-attachments/assets/6c09c563-4e01-459c-9915-b0e0c0d3a3e7" />

- CMOS inverter applied under various supply voltages

### L2: Advantages and disadvantages using low supply voltage

- Gain factor is the ratio of output voltage change to the input voltage

<img width="503" height="402" alt="image" src="https://github.com/user-attachments/assets/0bea1546-9e36-40a8-8abb-a3240054e5d0" />

- Energy = 1/2 CV**2
- By Operating at 2.5 V the then energy  will be 3.125*C
- By Operating at 0.5 V the then energy  will be 0.125*C
- The gain in the energy is 96% (reduction of energy by using 0.5 V from 2.5 V)

- The rise delay is 66 ps and the fall delay  is 78 ps (while CMOS inverter is  operating at 2.5 V)
- while CMOS inverter is operating at 0.5 V. this supply is not enough
- The device is not able to charge(rise time is not sufficient) andn completely discharge
- Device which is operating at 0.5 V need to perform the same operation like 2.5 V. Need extra rise time

- The rise delay is 220 ps and the fall delay  is 265 ps (while CMOS inverter is  operating at 0.5 V)

<img width="422" height="307" alt="image" src="https://github.com/user-attachments/assets/bff3c728-8318-4357-a02c-75e84fef42d5" />

### L3: Sky130 Supply Variation Labs

<img width="501" height="406" alt="image" src="https://github.com/user-attachments/assets/5341eeca-421b-46ee-8595-1c289e5e871a" />

<img width="502" height="405" alt="image" src="https://github.com/user-attachments/assets/d62eab0b-7131-4d6a-942d-5d46d3870c19" />

- By following the  instructions

<img width="527" height="407" alt="image" src="https://github.com/user-attachments/assets/4cd3f83f-e735-4fe8-ad06-96a2280e0697" />

- Here the Plot for Differnet Vdd and same W/L PMOS to NMOS

<img width="606" height="458" alt="image" src="https://github.com/user-attachments/assets/4b128b06-6d94-49f4-bf4d-5661abd0ce31" />

-  Here the Curves of VTC plotted and ranging from 1.8 V to 0.8 V
-  Gain factor is the ratio of output voltage change to the input voltage change.

#### Gain for Curves

-  For VTC 1.8V  curve
  
<img width="401" height="306" alt="image" src="https://github.com/user-attachments/assets/aab6ce07-4ba4-4ac4-ad4d-cd5cc362841a" />

- First seperate Y-Values = 1.718 - 0.129 = 1.589
- First seperate X-Values = 0.965 - 0.760 = 0.205

- The ratio of change in Y- Values to Change in X- Values is known as **Gain = 7.751**

-  For VTC 1V curve

<img width="396" height="303" alt="image" src="https://github.com/user-attachments/assets/5d0404e4-2119-46e1-80c9-9f7abad6d473" />

- First seperate Y-Values = 0.963 - 0.036 = 0.927
- First seperate X-Values = 0.577 - 0.488 = 0.089

- The ratio of change in Y- Values to Change in X- Values is known as **Gain = 10.921**

-  For VTC 0.8V curve

<img width="404" height="301" alt="image" src="https://github.com/user-attachments/assets/3022d946-f9a5-4d46-80ac-dc1e6d6306fa" />

- First seperate Y-Values = 0.774 - 0.025 = 0.749 
- First seperate X-Values = 0.509 - 0.417 = 1.22

- The ratio of change in Y- Values to Change in X- Values is known as **Gain = 0.613**

- Here gain keep increasing while operating  1.8V VTC curve decreasing until 1V VTC curve(i .e inversly propotinal )
  
- Here gain keep decreasing while operating 1V VTC curve to beyond 0.8V VTC curve (i.e is because to supply Voltage is not enough to drive the PFET and NFET transistors

## Static behavior evaluation – CMOS inverter robustness – Device variation
### L1: Sources of variation – Etching process

#### Single Inverter
-  Layout view
- Mental lines
- Blue - metal layer ,
- Green - P diffusion
- Yellow - N diffusion
- Red- polysilicon
- Black cross is the contact
- L is the Gate lenght at which node/technology you are(20nm,25nm.....)
- W is the Width . it identify overlap area of P diffusion

<img width="500" height="406" alt="image" src="https://github.com/user-attachments/assets/ab2ad38c-342b-4225-b594-333d1d87d188" />

#### Inverter Chain

- Ideal Mask (Area = W * L) and Actual Mask (Area = W′ × L′)

<img width="509" height="400" alt="image" src="https://github.com/user-attachments/assets/6ceb1df8-889a-4f7f-9e87-79ea13947647" />

- Due to diffrent processes involved in the FAB

<img width="500" height="403" alt="image" src="https://github.com/user-attachments/assets/e8a4566c-21b3-4855-97bd-76ed12402825" />

- Drain current is Directly related to the (W/L) it will causes impact of the Delay

<img width="507" height="401" alt="image" src="https://github.com/user-attachments/assets/ad3195a8-324c-4e7b-975f-06413023b907" />

### L2: Sources of variation – oxide thickness

- Now we are looking cross sectional view of the transistor

<img width="502" height="403" alt="image" src="https://github.com/user-attachments/assets/37de8281-377c-4749-84e4-806ee38f2d06" />

#### Ideal vs Actual Oxidation Process

- Due to FAB involved with many chemical process. the Oxidation thickness changes from ideal case
- Throughout the channel there will oxide thickness change


<img width="500" height="405" alt="image" src="https://github.com/user-attachments/assets/5ffc39e9-970a-4d35-80d1-1a8d9da72b9b" />

- Oxide thickness (Cox) = εox / tox

- More Oxide thickness variation more Id current variation (directly proportional)

<img width="401" height="300" alt="image" src="https://github.com/user-attachments/assets/3150a531-3403-4f7b-ae8e-4ba8b89af810" />

### L3: Smart SPICE simulation for device variations

#### Strong PMOS (Wp = 1.875µ) and Weak NMOS (Wn = 0.375µ)

- Increase the Size of the PMOS then the resistance going to reduce as the result of that it is called Strong PMOS and contravary for the NMOS 

##### Weak PMOS (Wp = 0.375µ) and Strong NMOS (Wn = 1.875µ)
- If the Voltage is given then NMOS is active
- Here we able to Sweep the Width 

<img width="501" height="405" alt="image" src="https://github.com/user-attachments/assets/d75ba126-3934-40ac-99f6-c205bbf44925" />

- here is the  CMOS inverter Robustness

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/b13603f9-f6c6-44c1-a5b7-aba27950a618" />

### L4: Conclusion
- By drawing a line and making an angle 45 degress with X axis
 
- We are getting Vm shift (0.7 V to 1.4 V)

<img width="500" height="407" alt="image" src="https://github.com/user-attachments/assets/420b2c51-2521-4c3f-b2b8-73e49f0062f7" />

- Varitions in the noise margin  (NMH - 2.1 V to 2.4 V) and (NML - 0.19V to 0.28V)

<img width="504" height="406" alt="image" src="https://github.com/user-attachments/assets/60dce810-f4e5-41dd-bd15-49edab560899" />

- Operation Of Gate is Intact
- In Dynamic waveform varies with respective time.

### L5: Sky130 Device Variation Labs

<img width="501" height="404" alt="image" src="https://github.com/user-attachments/assets/cb636dd7-8052-488f-9df2-2b90ebf34ea9" />

- Here, huge holding on Vdd  for longer duration compare to the NFET ,  
- IN this VTC curve Output holds the curve for long duration compared to the ground
- i.e  we tends to increase the width of the PFET is very high
- Drive strength of the PFET increase

<img width="600" height="457" alt="image" src="https://github.com/user-attachments/assets/2f97cdfc-3b98-4148-8a57-aa3f92261142" />

- At Vdd / 2 Switching Happens in ideal case
- CMOS is Robusted

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/5e84f50a-bd3d-4448-a457-1716efc6ebde" />

## Conclusion and Opinion

During the course, I explored MOSFETs and CMOS inverters in detail, learning how inverter characteristics can be modified and how to create a SPICE deck from a netlist for simulation. I studied CMOS voltage transfer characteristics, the factors influencing them, and methods for static behavior evaluation. The lab activities were especially insightful—the plots generated encouraged me to experiment with parameter changes in the SPICE code. Overall, the workshop sparked my interest in mastering MOSFET fundamentals and provided a rewarding experience with VLSI System Design, supported by constant guidance throughout.


# References

- [https://github.com/kunalg123/sky130CircuitDesignWorkshop](https://github.com/kunalg123/sky130CircuitDesignWorkshop)
- [https://www.vsdiat.com/](https://www.vsdiat.com/)
- [https://github.com/kunalg123/vsdflow](https://github.com/kunalg123/vsdflow)
- [https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [https://docs.github.com/en/github/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables](https://docs.github.com/en/github/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables)









































































 



























































  












  













