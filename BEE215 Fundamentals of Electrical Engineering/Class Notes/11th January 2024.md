The relationship between Voltage and Current is linear, and this is saying across a resistor; since its a passive device.
#### k - conductance
k is the conductance.
Mhos = Siemens; which is just Ohms backwards

Conductance goes up, resistance goes down

#### Resistors follow passive-sign conventions
They cannot generate energy; supply - they can only absorb it.

**Noteworthy to memorise:**
- p = i^2 * R
- p= (v^2)/R

##### "I don't think my whole life I've ever done this calculation"
- Gv^2

##### Independent Sources
It has no depdencies (maybe aside from the actual adjustable knob)

##### Dependent Sources
Voltage source or Current source that depends on another value of source inside another circuit
*The behaviour of a source on how much voltage or current is outputted is dependent on somewhere else in the circuit
**Dependent Sources; Mathematically, generate power!**

##### The voltage source
Battery, chemical reaction -> outputs a voltage. Simple
##### The current source
Will supply a fixed amount of current, independent of the voltage across it.
It will be whatever it needs to be; so that it flows what it needs.
- The voltage across the current source is determined by the rest of the circuit
	- Necessary to be adjusted to maintain the constant current source value.
***Real World - Siglent SDP1305X
The Power Supply**
*In an idea current source, it will generate as much voltage as needed to contain a consistent current*

### There are four basic types of dependent sources
**CCVS, Current Controlled Voltage Source**
- Source voltage *vd* is a function of a control current *ic* flowing somewhere else in the circuit *r* is called the gain.
- *vd* = *r* * *ic*
**VCVS, Voltage Controlled Voltage Source
VCCS, Voltage Controlled Current source**
**CCCS, Current Controlled Current Source
- This one is the closest to actual transistors on how they work
- The current, somewhere in the circuit, is adjusted by the gain.
#### Independent Source Examples
![[Pasted image 20240111133517.png]]
##### Current Flow
Is arbitrarily assigned.
- If built in LTSpice, we would have an inverse of a design
![[Pasted image 20240111133835.png]]
#### Noting the polarity (Figure Above)
The positive point, would be like saying you set your red-lead on the higher point.
And the negative point, the black-lead would be left on the lower point.
Regarding that (- -> +) black to red.

##### Is there no way to get negative power?
**Negative Power** that a source produces is being sucked in from the environment; somehow. So it's the "Absorption"; which is negative power
**Positive Power** is when energy is radiated back into the environment.
*In regards to a resistor, there is no way to generate negative power through a resistor because it will never get cold, even if we set a negative current flow through it*

#### Transistor
![[Pasted image 20240111134630.png]]
![[Pasted image 20240111134534.png]]
*It is an active device*
C, B, and E.
By doing something to 'B' terminal, we can do something to that entire terminal

By producing a current to flow through the **B** terminal, it causes a current to flow through the loop of **C; collector** to **E; emitter**.
*Context: For this transistor circuit, the current-source is ideal*

**The line is kind of misleading** since both sides are abled with the same voltage
The current that flows in either loop are independent of each other.
### A more accurate model of a Transistor
![[Pasted image 20240111135131.png]]
The current from collector to emitter is equal to 'Beta' multiplied by whatever current is flowing through the **Base (B)**. *In this context: In order for current to flow through the Base, you must have a voltage that exceeds 0.6V*
"Kirkland brown bag Beta is 100"

## In-class Problem
![[Pasted image 20240111140035.png]]
#### Context for the arrows
![[Pasted image 20240111141729.png]]
Represents an arbitrary fuck-off direction somewhere in space there's a 5V source.
![[Pasted image 20240111142404.png]]
**Figure redrawn for context**
### Strategy:

##### The first reference point @ 5V
1. Finding the voltage drop across the 10K Ohm Resistor:
##### Measuring the reference across the Emitter (E) and Collector (C)
Would be 10.5V

#### "The funny lil' symbol" is ground.
![[Pasted image 20240111135509.png]]
#### Diode
![[Pasted image 20240111134654.png]]


## Footnote:
##### Fall in love with transistors.
