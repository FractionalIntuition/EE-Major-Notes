# States of Diodes
## Review
The typical impression of a diode being "on" are a diode who's $V_I$ to a Diode's *entering* node. The voltage limit across the diode is 0; because there is an absence of a voltage drop.
![[Pasted image 20240701083701.png]]
![[Pasted image 20240701083757.png]]
When placed on a graph of a voltage over time; the $V_o(t)$ for an ideal diode.

$V_I(t)=V_Psin(\omega t)$
When presenting a diode; the ***transfer function*** of a diode concerns itself with being $V_I>V_On$
![[Pasted image 20240701084104.png]]
When reversing the polarity of a diode, the effect it has is that it loops the diode's limit and instead works towards a minimum.

Us having a control over the threshhold voltage to turn "on", we have full control over the voltage continuation after the threshhold has been reached.

## Ex 1
![[Pasted image 20240701084502.png]]
Remember conditionals
![[Pasted image 20240701084615.png]]
![[Pasted image 20240701084738.png]]
## Presuming ON
![[Pasted image 20240701084958.png]]
![[Pasted image 20240701085027.png]]
### Simplified Strategy:
Sometimes we just need to select a reduced version of the slope; where we pick an arbitrary spot, and just connect the points.
## Limiting over lower boundaries
![[Pasted image 20240701085425.png]]
### When given a transfer curve, we find the limit voltage:
![[Pasted image 20240701085542.png]]
We should be able to find the sinusoidal limits of the curve over time
![[Pasted image 20240701085837.png]]

## In-class Participation Part 1
## A load line of a diode is the same as the diode of the curve
### *No*
![[Pasted image 20240701090536.png]]
Emphasising the difference across the Diode; with the relationship relative to $V_D$ and $I_D$ over a Exponential circuit involve a series $V_S$, $I_D$, and $D$.
**Load Line:** always $y=-mx+b$, a declining slope; and represents the linear behaviour of the circuit without the diode - essentially the voltage decline over the declination of the voltage.
**Diode Curve:** is the relationship of the circuit's behaviour with the inclusive the diode.

## Essentially Thevenin's Equivalent
Realise the complication of the a simple VRD circuit; is the portion of the 

The diode would regulate the upper voltage; noting that the Diode; when it turns on. The output voltage $V_o$ will equate to $V_{on}$
![[Pasted image 20240701091041.png]]
### Increasing the multiplicity of the output voltage
Essentially scales to the $V_o$ of how many diodes in series there are to the respected regulating branch of diode
![[Pasted image 20240701091221.png]]
# The behaviour of a VRD circuit
![[Pasted image 20240701091816.png]]
## Zener \& Normal Diode
![[Pasted image 20240701092144.png]]

## Zener Diode Analysis
![[Pasted image 20240701092915.png]]
The regulation of the output voltage of a Zener diode; the percent err we're concerned with aren't typically is given the behaviour of the above.
## The Zener Diode Graphical Segments
## Memorise this shit. Lmfaaaaaaoooooooo
### Context Circuit:
![[Pasted image 20240701093659.png]]
### Forward Bias
- $I_D>0$
- $V_D=V_{ON}$
![[Pasted image 20240701093244.png]]
### *Off* Portion
- $I_D=0$
- $-V_{Z_o}<V_D<V_{ON}$
![[Pasted image 20240701093339.png]]
### Reverse Breakdown Region; RBR
- $I_D<0$
- $V_D< -V_{Z_o}$
![[Pasted image 20240701093604.png]]
## Zener Diode Characteristics
- 3 segments
	- Forward Bias
	- Cut-off
	- Reverse Breakdown
- Typically used for the reverse breakdown portion of the circuit; to regulate the negative portion of the diode.
![[Pasted image 20240701095124.png]]
![[Pasted image 20240701095522.png]]
- Characteristics must be known; the turn on voltage: **CVD**
	- We must be presented with the candid value; as the form of **CVD: $V_{ON}$**
	- Or the graphical value; presented as the ideal graphical curve @ a point
![[Pasted image 20240701095921.png]]
We have presented above an ideal Zenode Diode; which are realising *this is an extremely good Zenode Diode*

## Typical presumption for a Zenode Diode
### Just assume R.B. Lmfaaaaaooooooo
- $I_D < 0$
![[Pasted image 20240701100754.png]]
## *Tangent: 215 Review*
![[Pasted image 20240701100346.png]]
The function of a generator; these wattages - they step up the voltages; and the potential current can also increase. It will *generate*, power.
- Positive Wattage: $P>0$, Absorbing Power
- Negative Wattage: $P<0$, Delivering Power
![[Pasted image 20240701100540.png]]
*Tangent End*
## Typically assume; then verify through graphical functions
![[Pasted image 20240701100908.png]]
## Current
![[Pasted image 20240701100957.png]]
![[Pasted image 20240701101610.png]]
### Assumption Forward Bias
Assume $I_D > 0$
![[Pasted image 20240701101843.png]]
### Assumption Cut-off
If the Zenode Diode cut-off, verify between the two boundaries of $V_D$
![[Pasted image 20240701102101.png]]
# Zener Diode Review
![[Pasted image 20240701103218.png]]
- Characteristics of a Zenode Diode are built into the diode; by schematic
- The resistance of the Zenode Diode should be observed and considered in the schematic
## Two Zenode Diodes
![[Pasted image 20240701103318.png]]

# Ex 3; RVD: Where R is not 0
![[Pasted image 20240701104015.png]]
## Useful usages of the Zener Diode
When the Zener Diode is in *Reverse Breakdown*, it becomes a great voltage regulator.
# Ex 4; RVD
![[Pasted image 20240701104439.png]]
REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN REVERSE BREAKDOWN 
![[Pasted image 20240701104826.png]]
The smaller $R_L$ is, the more likely that the diode characteristics of the regression will lower
![[Pasted image 20240701105149.png]]
## Conditions that the Zenode Diode would operate in cut-off
Is when the $-V_D$ limit equates to the $+V_D$ over the $V_D$ line.
![[Pasted image 20240701105531.png]]
As $R_L$ changes, and your Zenode diode still operates in *Reverse Breakdown*. Then your output voltage would operate between the boundary the *Reverse Breakdown Cut-off* to *Cut-off "Off"*. 
![[Pasted image 20240701105811.png]]
![[Pasted image 20240701105859.png]]
## Fast $R_{L_{min}}$ Discovery
![[Pasted image 20240701110137.png]]

# Reminder: Summer, we move fast.
## Review Frequently
## Duration of study should be relevant
## Be efficient
## Be good at memorising

