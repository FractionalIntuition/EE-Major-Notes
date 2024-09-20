# Diodes
- Exponential
	- No assumptions, just solve.
	- Most accurate
- ***Ideal***
	- Presumptions made; On or Off
	- Most efficient; least accurate - sacrifices a lot of precision
- ***CVD***
	- Presumptions made; On or Off
	- Best balance

# Ideal Diode Model Calculations

Realise if the Diode is either on or off.

Assuming whether the Diode is on or off, and checking whether your assumption is correct or not.
	So thusly, we verify

We do not assume voltage drop across the diode;
- **Reason:** the instances of the answers being inaccurate; the Ideal model creates an easier nodal analysis while also sacrificing a lot of precision.
## Characteristics of an On/Off Diode
### On
- Current is positive; $I_D > 0$
### Off
- Voltage is negative; $V_D < 0$

# Diode operating (Q) point Q($I_D$, $V_D$)
- In given example: $Q(0A,-5V)$
![[Pasted image 20240624090030.png]]

# Example 2
## Differences in voltage @ polarity of Diode
![[Pasted image 20240624090258.png]]

# Definition of polarity reference to the voltage source
Differences between the polarities of *high*; positive, to *low*; negative.
- Specifying something as "reference" is 0V; grounded
How to instantaneously determine what is "high" to "low"?
- It's the status of the **Voltage _Drop_**
Node voltage; typical of reference point. 
![[Pasted image 20240624091106.png]]
# Best Practise; "Typical Plan of Attack" to solving Diodes
1) Make a reasonable assumption
	1) Short-circuit the diode
		1) Calculate for $I_D$ across the short-circuited Diode
			1) Verify if $I_D>0$
				1) **If true:** The voltage is 0; $V_D=0$
				2) **If false:** $V_D>0$
	2) Open-circuit the diode
		1) Calculate the $V_D$ across the open-circuited Diode
			1) Verify if $V_D<0$
				1) **If true:** The current is 0; $I_D=0$
				2) **If false:** $I_D > 0$
2) Solve
3) 2
4) Verify
5) Final answer in the form of $Q(I_D,V_D)$
# Have strong fundamentals
## Basic skills about Ohm's Law; KCL; KVL
### Review: What is a linear circuit element?
- When a circuit element or a variable is dependent on another element or variable
**Elements include: **
- Voltage source
	- Dependent
		- *Can be*
		- e.g. $X^2$; Non-linear
	- Independent
- Current source
	- Dependent
		- *Can be*
		- e.g. $X^2$; Non-linear
	- Independent
- Resistor
- Capacitor
- Inductor
# Constant Voltage Drop (CVD): Diode Model
1) Assume that there is a constant voltage source.
	1) Reviewing the exponential mode; analyzing after some point, the exponential voltage point starts to plateau. The $V_D$ doesn't change all that much in the model after a certain point of $V_T$. $I_D$ will change in great magnitudes until those points.
# Review; Week 1: Exponential Model
## $I_D=I_S(e^{\frac{V_D}{V_T}}-1)$
- Most accurate

# Choi's tangent about his research
## Voltage across a diode
- If the material given arbitrarily; can seemingly be 0.7V
- If the material is a semiconductor; the voltage across the diode would have a voltage transience of 0.7V's *range*
- Silicone diode; arbitrarily turns on @ 0.7V
- And say we have a different diode; dominion diode
	- Different diodes have different diode characteristic curves
## Exam tips
- He will have a given type of voltage; and he will be given voltages.
- "I will be the one who tells you what number to use"
	- In a real-world setting; we look at the ideal of the material of the voltage.

# Graphical Methode
(Choi is French)
Similar to how the exponential methode utilises two equations; one for the voltage across the linear voltage circuit; KVL. And the second equation being the equation across the diode.

The graphical methode utilises *two graphs* in lieu of a *two equation methode*.

## Context for the linear portion; slope (Load-line):
It represents the circuit-behaviour not inclusive to the exponential portion of the graph; the diode. $I_D=-\frac{1}{R}*V_D+\frac{V_S}{R}$
## Context for the exponential portion:
The entire circuit; with the context of the diode that is involved. Different diodes have different diode curves; so arbitrarily the intersection; **Q*** will change.
## When using the ideal diode models
We change the diode curve to the *Ideal* diode curve. 
- Not an exponential curve; but instead a sharp voltage; *IMPULSE* voltage pique @ $V_D$
*Q will never be the same as your CVD*
### Prefer to use CVD to substitute
# He won't ask us to graphical methode using the exponential diode model
# Efficient method of finding the Load-line for the Graphical Methode
## Find the axises
$I_D @ V_D=0$
$V_D@I_D=0$
### So we substitute the circuit's values; as "known" values of 
- $V_D=0$; OPEN THE CIRCUIT DIODE
- $I_D=0$; SHORT THE CIRCUIT DIODE
### Then connect the two points together.
### Now, we just find $Q(I_X,V_X)$
