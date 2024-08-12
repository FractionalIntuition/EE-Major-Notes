# Best Practises;
- Draw the circuit
- Sample if we
	- 1) Know $V_G$ & $V_D$
	- 2) Then see if we can use the Saturation Equation
		- $V_{GS}-V_{tp}\geq V_{DS}$
	- 3) Utilising the $I_D$ equation;
		- $I_D=k_{n/p}(V_{GS}-V_{tp}-\frac{V_{DS}}{2})V_{DS}$
		- Results in a quadratic equation; choose the relevant answer based on Saturation or Triode.
	- 4) Confirm or Deny
First see, if the variables are available in the circuit; and determine if they're saturation or triode.
![[Pasted image 20240731084641.png]]
# Remember the mantra
## "Simple, not easy"

# In the context of a switch, is there a distinction between a CMOS and a NMOS/PMOS Switch
![[Pasted image 20240731085257.png]]
For the transition of a triode to cut-off range for a MOSFET, the context lies in the necessity to pass through the saturation region regardless; however, we aim to minimise the duration in a saturation-stage.
# Today's Lesson Plan:
## Logic
Ideal case, all logic gates occur at the same time.
However, realistically, there will be a delay; see below
![[Pasted image 20240731085847.png]]
In a true-case; we would utilise a clock-signal to synchronize the logic gates. We're waiting for the clock signal to essentially handle the signals for the entire system; however, when we generate a clock signal - it will rely on the slowest rate of delay (50ms). Due to the required delay to have the "Next Universal Cycle" that only syncs at the slowest-rate-delay.

*So, do we make the clock faster?*
![[Pasted image 20240731090533.png]]
*We do not make the clock faster; however, we can lower the delay propagation - by designing a transistor.*
So we address the propagation-delay directly by manufacturing or designing a better MOSFET.
# Example
![[Pasted image 20240731091132.png]]
## Reference Inverter; Logic Gate for X
![[Pasted image 20240731091149.png]]
## Logic Gates for Y
![[Pasted image 20240731091232.png]]
![[Pasted image 20240731091457.png]]
## Truth Table
![[Pasted image 20240731091939.png]]
## Propagation Delay
The realistic context to propagation delay is $\tau_p,ref$ as the propagation delay. In a realistic context; we will always have a change over a duration of time ($\tau$)
## Logic Gate Circuit Diagram
![[Pasted image 20240731092259.png]]
### Fully-charged?
- RC-time constant
@Reference Inverter (X)
![[Pasted image 20240731092411.png]]
@Logic Gate $\overline{B+CD}$ (Y)
![[Pasted image 20240731092512.png]]
If it turns on, then it can be represented as "Channel Resistance"; $r_{DS,ref}$ @ the **NMOS** side of the circuit.
![[Pasted image 20240731092620.png]]
![[Pasted image 20240731092758.png]]
## Fully context mathematically
### Ref Inverter
$\tau_{p,ref}\propto r_{ds,ref}*C_{DD}$
### Logic for y
$\tau_{p,new}\propto(r_{ds,c}+r_{ds,D})*C_{DD}$
![[Pasted image 20240731093142.png]]
### Manipulating the value of $r_{ds}=\frac{V_{DS}}{I_D}=\frac{1}{k_n(V_{GS}-V_{tn})}$
$I_D=k_n(V_{GS}-V_{tn}-\frac{V_{DS}}{2})V_{DS}$
Thus,
$r_{DS}\propto\frac{1}{k_n}\propto\frac{1}{(\frac{W}{L})}$
So, the reference resistance is inversely proportional to the $\frac{Width}{Length}$

*Example of $r_{DS,C}$*
![[Pasted image 20240731093520.png]]

# The job of a design Enjunear
![[Pasted image 20240731094050.png]]
### 1) Establishing the Width/Length of the NMOS & PMOS
![[Pasted image 20240731094122.png]]
### 2) Designing the Circuit Logic Design
![[Pasted image 20240731094256.png]]
### 3) Specifying the MOSFETs
- Context here for NMOS
![[Pasted image 20240731094417.png]]
### 4) Finding the PMOS Equivalent
### 5) Finding the same propagation delay $\tau_{p,ref}=\tau_{p,new}$
- 5a) Understand that: ![[Pasted image 20240731094625.png]]
- 5b) Finding the longest path, "Worst-case Scenario" for propagation delay:
	- $r_{ds,ref}*C=(r_{ds,A}+r_{ds,C}+r_{ds,D})C$
	- $R_{DS,ref}=3r_{ds,A}$
		- Assuming $r_{ds,A}+r_{ds,C}+r_{ds,D}$
	- $\frac{1}{\frac{W}{L}_ref}=3\frac{1}{(\frac{W}{L})_A}=3*5=15$
![[Pasted image 20240731095015.png]]
![[Pasted image 20240731095323.png]]
## Context:
**Your customer** desire a propagation delay of $0.5\tau_{p,ref}=\tau_{p,new}$

$0.5\tau_{p,ref}=\tau_{p,new}$
$0.5(r_{ds,ref}*C)=(r_{ds,A}+r_{ds,C}+r_{ds,D})*C$
$0.5(\frac{1}{\frac{W}{L}_ref})=3\frac{1}{(\frac{W}{L}_A)}$
$=>\frac{W}{L}_A=\frac{W}{L}_C=\frac{W}{L}_D=\frac{3}{0.5}\frac{W}{L}_{ref}=6*5=30$
![[Pasted image 20240731095752.png]]

**Another customer** desires a 3 times larger capacitance, $3C$.
![[Pasted image 20240731095907.png]]
![[Pasted image 20240731100159.png]]
Designing engineers, just need to design the circuits; delayed propgation - the design engineers just put them together. The manufacturers have already made the component with its contextual component schem.

**After designing the circuit with the ideal propagation**, we include the clock signal to avoid the glitches; and properly sync them to the *"Next Logic"*.

## For a design engineer,
We should

N->Y->P
Y->N->P
P->N->Y

Once we design the logic-gate, we should be able to design the transistor size.

# Rest of Coverage
## BJT 
### Today & Next Week
## Semiconductor Physics
### Next Week
#### One conceptual question; VERY BRIEF
## Final Exam Review

# Bi-junction Transistor (BJT)
## I'll miss you CE majors
The nature of a Transistor is often for switching or amplification. As the BJT, it is fundamentally a charge carrier for both Electrons and Holes. Typically, you'll find a BJT as an amplifying element; component.

## NMOSFET
![[Pasted image 20240731102335.png]]

## Bipolar
Electrons and Holes carrier
![[Pasted image 20240731102615.png]]
### Circuit Diagram
![[Pasted image 20240731102900.png]]


### How to use a BJT for its intended design
![[Pasted image 20240731103528.png]]
![[Pasted image 20240731103534.png]]
### Periodic Table
![[Pasted image 20240731103706.png]]
![[Pasted image 20240731103712.png]]
The typical silicone diode has a body of 99% Silicone. And the chemically stable Silicone structure takes place towards the next available electron; which is each other. 
![[Pasted image 20240731103844.png]]
We take the silicone structure and heat it to a ridiculously hot standard, and then we re-arrange the bonds it has, and entails a crystalline structure.
Even if we combine the two ends of this silicone diode after construction, we shouldn't expect change: ![[Pasted image 20240731104110.png]]

![[Pasted image 20240731104521.png]]
## Natures of P-side and N-side
### "Diffusion"
![[Pasted image 20240731104929.png]]
Whenever you see the N-Type, just presume there are an abundance of electrons, and between P-side, Boron is in abundance with P-type (positive) holes$^+$.
![[Pasted image 20240731104918.png]]
![[Pasted image 20240731105255.png]]
Due to the context of Boron losing electrons; the Boron becomes more positive, and post-diffusal with Silicone; the post-haste of the negative charge in conext of diffiusal.
![[Pasted image 20240731105457.png]]

The abundance of holes and the abundance of electrons when the increasing and lower of polarities finally settle, you lose current, with $i\frac{dq}{dt}$
![[Pasted image 20240731110130.png]]
With the large abundance of electrons and holes, the Voltage difference @ the $V_{out}$.

