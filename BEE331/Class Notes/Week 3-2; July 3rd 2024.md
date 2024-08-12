# Zener Diode
![[Pasted image 20240703083955.png]]
![[Pasted image 20240703084157.png]]
Commonly we try to approach a system that is commonly non-linear, our goal is to tackle the circuit and manipulate the characteristics to linearise the circuit.

## Cut-off
![[Pasted image 20240703084329.png]]
## Reverse Bias
![[Pasted image 20240703084522.png]]
"What is the voltage across $V_D$"; so given the circuit - the theoretical equation would just be:
$V_{Z_0}+I_Z+r_z=-V_D=V_Z=V_{Z_0}+(-I_D)r_Z$

Essentially, our goal is just to substitute the Zenode diode into typical linear circuit components; which we then practise fundamental circuit analysis techniques.

### Choi's Fabrication Tangent
The fabrication of various Zenode diodes deviate by small degrees - when recognising the natural curve of a Zenode diode - all engineers interpret the data differently.

The data sheet commonly utilise a test current, noted as $I_{z_t}$
- The data sheet would also document the data's Q point as ($I_{Z_T},V_Z$)
	- Remember $I_{Z_T}=I_D$
	- Remember $V_Z=V_D$
![[Pasted image 20240703085728.png]]
In a lot of our future of circuit analysis - we have a lot of design considerations to be made. And a lot of the time, it's up to us for interpretation.
![[Pasted image 20240703090013.png]]
The diodes are commonly transistors and junctions shown be conductive at various different temperatures. The material being temperature dependent, can also generate a lot of heat.

Due to the temperature considerations and inconsistencies of semiconductor materials, voltages were commonly transient. Because of this, Germanium diodes were replaced with high priority because of their temperature; even if they were the most utilised.

Silicone doides. ![[Pasted image 20240703090325.png]]

## In-class quiz
![[Pasted image 20240703091205.png]]
## References to Sinusoidal Voltage
- $V_{RMS}$
- AC to DC transformation
- Voltage step-down transformer
![[Pasted image 20240703092148.png]]
### Keeping only one polarity of AC signals
We utilise a diode to maintain a one-sided polarity of the AC signal.
![[Pasted image 20240703092453.png]]
For the above circuit, let's presume an ideal diode.
- Ideal: There is no voltage drop
## Sinusoidal Representation of IDEAL diode
![[Pasted image 20240703092748.png]]
## Substitution of resistor with capacitor
![[Pasted image 20240703093811.png]]
# In-class quiz 3
![[Pasted image 20240703095405.png]]

## Introduction to Diode Source-free RC Circuit
![[Pasted image 20240703100610.png]]

![[Pasted image 20240703102005.png]]
When increasing the RC constant; the trade-off is that the capacitors are fucking massive.
![[Pasted image 20240703102123.png]]
![[Pasted image 20240703101518.png]]
![[Pasted image 20240703102703.png]]
We also need to consider frequency of the Voltage Source when creating a parameter for the RC circuit equation
- As we're in AC circuit; $V_o(t)=V_p(e^{-\frac{t}{RC}})$
	- The characteristic of time is determined by Frequency
	- The characteristic of time-constant; TAO, is RC
## Decreasing the ripple voltage
- the utilisation of the Zener diode when its in the R.B.
![[Pasted image 20240703103316.png]]
## Utilising a CVD diode for a AC Source RC Circuit
![[Pasted image 20240703105503.png]]
As a result of the DVRC circuit; we should have a very brief period where the Diode is actually on. Otherwise, the RC circuit would sustain a Diode with a value that's below CVD; so - "off".
## Taylor Series Review
We actually use ALL the fucking math we have
![[Pasted image 20240703110035.png]]
 ![[Pasted image 20240703110504.png]]
 If the circuit is good enough; the $\frac{\Delta T}{RC}$ is neglible ![[Pasted image 20240703110543.png]]
 ![[Pasted image 20240703110659.png]]
 Manipulating the overall equation; is where we can actually change a non-constant variable; which is $\tau$ (RC)

### Closing note
The only time we can utilise this theoretical equation is when we make $\tau > T$; Time of RC larger than the period of Time.