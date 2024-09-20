# HAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAHAAHAHAHAHAHAH DEMORGAN HHAHAHAHAHHAAHA DEMORGAN
# 271 Review

## Boolean Logic Gates
![[Pasted image 20240724085508.png]]
## Demorgan's Theorem
![[Pasted image 20240724090014.png]]
## NOR or NAND exclusive
![[Pasted image 20240724090249.png]]
![[Pasted image 20240724090437.png]]


# THE BUBBLE JASON
# THE BUUUUBBBLE
![[Pasted image 20240724085307.png]]

# Quiz
## What are the two conditions for MOSFET Linear Amplifiers?
Saturation Region and small voltage input.

# Returning to topic; Demorgan's
![[Pasted image 20240724091441.png]]
## MOSFET; NMOS Inerter
![[Pasted image 20240724091534.png]]
When the Transistor is *on*, current flows, if the Transistor is *off*, the current doesn't flow.

![[Pasted image 20240724091720.png]]
![[Pasted image 20240724092106.png]]

The relationship between $V_{DS}$ and $V_{out}$, inversely proportional to each other. As $V_{out}$ exponentially gets closer and closer to 0.
![[Pasted image 20240724092443.png]]
![[Pasted image 20240724092448.png]]

## Relationship with Power
![[Pasted image 20240724092618.png]]
In the case of a Transistor being in its "high" state, would dedicate too much power in consumption (the minimum power) when sitting above the threshold - is commonly an issue amongst portable electronics due to the "passive consumption" of the apparatus.

## MOSFET; CMOS Inverter
The "C" in CMOS is defined as complimentary MOSFET

So when NMOS is on, the PMOS is off - and vice-versa.
![[Pasted image 20240724093537.png]]
![[Pasted image 20240724093544.png]]
## When $V_{in}=0$
### PMOS = ON
![[Pasted image 20240724093653.png]]
![[Pasted image 20240724093734.png]]
## When $V_{in}=V_{DD}$
### PMOS is OFF
![[Pasted image 20240724093946.png]]
## Summarising; full relationships
![[Pasted image 20240724094109.png]]
Operating both the NMOS and PMOS; the circuit prevents the passive power consumption from the direct current between PMOS; VDD -> VDS. It should remedy that issue due to creating a secondary; "**C**omplimentary" threshold.

## Space Issues
![[Pasted image 20240724094304.png]]

## Static Power Consumption = 0
## Switching (Dynamic) =/= 0
Changing the input voltage to half of $V_{DD}$, would cause the NMOS and PMOS to be *both on*, and current would flow all the way down from $V_{DD}$ to $Ground$. So we need to swing above, and below $\frac{V_{DD}}{2}=/=V_{in}$.
![[Pasted image 20240724094657.png]] 
# Steady Power Consumption
The ideal is to utilise a system without ANY passive power consumption; so essentially 0 steady power consumption. The few nanometres of CMOS circuitry should try to reduce that variable.

When the Transistors are "ON", they are in TRIODE operation range, and swings between saturation and triode operation ranges.
## CMOS Inverter Cont.
![[Pasted image 20240724100258.png]]
![[Pasted image 20240724100522.png]]
## To arrange and expand the CMOS Inverter
Just start stacking the fuck out of PMOS

## Pull-UP and Pull-DOWN Networks
![[Pasted image 20240724100815.png]]
The necessity of a NMOS and PMOS (Pull Down and Pull Up Network) would impede the Pull UP by cancelling it with Pull DOWN.

![[Pasted image 20240724101742.png]]

![[Pasted image 20240724102018.png]]
![[Pasted image 20240724102640.png]]
![[Pasted image 20240724102834.png]]
## Typically, you want your count of PMOS transistors to be proportional to your count of NMOS transistors
![[Pasted image 20240724103209.png]]
## Correct Parallel PMOS (I'm pepega)
![[Pasted image 20240724103608.png]]
# DEEEEEEEMORGAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAN
![[Pasted image 20240724103350.png]]
![[Pasted image 20240724103956.png]]
# Mathematically; the PMOS and NMOS Circuits are parallel to each other
![[Pasted image 20240724104219.png]]
### *Note:*
*Duality of * to +...*
![[Pasted image 20240724105126.png]]
## Typical Workflow
### When given NMOS First
- 1) Boolean Algebra of NMOS
- 2) Identify $Y$ output
- 3) Find PMOS; DeMorgan's (Overline)
### When Given PMOS First
- 1) Identify $Y$ output
- 2) Boolean Algebra of NMOS
- 3) Satisfy PMOS; (Double-Overline)
 . )