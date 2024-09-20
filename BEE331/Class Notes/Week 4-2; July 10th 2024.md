# Monday Review
Most metals have a lower melting points compared to typical processing; if it's lower than 1100C-1200C we cannot use the metal as a semiconducting material.

The metal simplifies these.

***Why can't we just structure the metal last?***
It's hierarchically structured in order of P-type; and the metal layer will be inbetween.

The Back-to-back diodes; we want to get rid of between the drain.
**The Source:** Connecting the body to the source
**The Drain:** The drains; respect to their sources - the same as the body
**The Gate:** We need the same type of charge carrier; the same as body of a threshhold.
- The gate has a certain potential to the source.

Essentially, source is in respect to body, and the further characteristics are in respect to **The Source**.

**NMOS; PMOS respectively**
![[Pasted image 20240710084320.png]]

# Continuation...
### Quiz: The threshold voltage of NMOS transistors are
*Positive.*
"This isn't something you memorise, this is something you try to understand."
- This should aide in more circuit analysis

There's counted 4 terminals; however, we incur 3-terminal transistors more frequently.

## Circuit Representation of NMOS
![[Pasted image 20240710085244.png]]
The terminals of the body shorting by the source; directs itself as an "off" for the Diode pointing to Source, and pointing to Drain.
The current representatively shows that $I_D =I_S$; Current Drain to Current Source.![[Pasted image 20240710085458.png]]
![[Pasted image 20240710085548.png]]
The "capacitance" factor we're looking at the mosfet is ENTIRELY DISREGARDED APPARENT-FUCKING-LY, so we're just having a straight current path going through the Drain to Source.

$Drain->Source$
![[Pasted image 20240710085843.png]]

## Connection between Drain and Source
The thin channel between Drain and Source; the electric carrier across the n-line is a resistive channel. If it were not resistive; with $0\Omega$, then this line is shorted - however there is an electrical carry between the two lines. So there is infact resistive channels.
![[Pasted image 20240710090107.png]]
![[Pasted image 20240710090117.png]]
## Voltage Drop across a transistor
The voltage terminals of Drain and Source, the difference between $Drain->Source$ have the difference denoted as $V_{DS}=V_D-V_S$. That is how we determine the voltage drop across the centre resistive line; denoted as $n$.
![[Pasted image 20240710090414.png]]
## Conduction between Ground and Drain
Occurs similarly to how a capacitor only occurs a current when there's an involvement of an AC-Signal the stead of a DC-Signal.

## 3-Terminal PMOS Transistors
![[Pasted image 20240710090817.png]]
The characteristics of a PMOS and an NMOS are very similar; and the only real differences are:
- Direction of current; PMOS v.s. NMOS
	- $Source->Drain$ v.s. $Drain->Source$
- P-Type vs N-Type
Otherwise, the attributes are the same and functionally act the same.
## Specificities of MOSFETs
### NMOS Focus
Denoting the voltage difference between Ground and Source is as $V_{GS}$. Being attentive to the conductivity across the transistor.
![[Pasted image 20240710091354.png]]
Due to the nature of $I_D=I_S$ across a transistor, we just denote the respective *direction of current* to it's equated opposing-terminal. 
![[Pasted image 20240710091514.png]]
The relationship between modifying the Drain Current, to the Source Current; it is denoted that the potential difference of $V_{DS}$ creates a current-channel over the thin resistive channel through the voltage difference of $V_{DS}$.

In laymen: The current of $I_D$ is proportional $V_{DS}$
![[Pasted image 20240710091822.png]]
Your resistance across the resistive line is dependent on the voltage of $V_{GS}$. Larger the ground, the resistance of the resistive-channel increases.
![[Pasted image 20240710092047.png]]
![[Pasted image 20240710092056.png]]
## Relationship between Holes and $V_{GS}$
![[Pasted image 20240710092212.png]]
The nature of holes push away further the higher $V_{GS}$ gets. So to say that $I_D$ is proportional to $V_{GS}-V_{TH}*V_{DS}$.
![[Pasted image 20240710092323.png]]
## Equation of Current: $i=\frac{dQ}{dt}$
## Recalling the linearity of Capacitance
"Higher capacitance, at a given voltage, will produce more charge."
![[Pasted image 20240710092620.png]]
### Relevant to a Transistor
The capacitor can be found between Ground and the substrate Body
![[Pasted image 20240710092809.png]]
### Physics II Throwback
![[Pasted image 20240710092949.png]]
![[Pasted image 20240710093054.png]]
- $A=Area$
- $\epsilon=Permeability$
- $d=Distance$
![[Pasted image 20240710093247.png]]
### So,
$C_{OX}$, Capacitance per Unit-Length; handles the Q of $dQ$ in $i=\frac{dQ}{dt}$
![[Pasted image 20240710093403.png]]
### Electrons vs Holes
![[Pasted image 20240710093426.png]]
As a carry-rate, electrons move a lot faster than holes. If you were to "race them", electrons would have a faster carry-rate overall.
### Galvin Arsenic; GaAs v.s. Silicone
The electrons in Galvin Arsenic move faster than Silicone.

### The measurement of electrons movement: MOBILITY; $\mu_n$
So, fully handling the proportional equation of Electrons Mobility handles the $dt$ time portion of $i=\frac{dQ}{dt}$

## The proportionality of Channel to $V_{GS}$
Innately, the two are the same...
Until the voltage difference across $V_{DS}$ begins to become diverse. So $V_D<V_S$
![[Pasted image 20240710094544.png]]
Graphically represented as:
![[Pasted image 20240710094805.png]]
Numerically represented as:
$\frac{V_{GS}-V_{TN}+V_{GS}-V_{TN}-V_{DS}}{2}$=$\frac{2(V_{GS}-V_{TN})}{2}-\frac{V_{DS}}{2}$

## Channel Length
the channel length in the depth between the two differences, the channel essentially changes its geometry around the "W" and "L"
![[Pasted image 20240710095140.png]]
- "L" being the length of the channel
- "W" being the depth of the channel and fabricated semiconductor
## Full Proportionality of $I_D$; NMOS
![[Pasted image 20240710095526.png]]
In laymen, reference to $NMOS; Drain->Source$
The Drain current is proportional to the **Proportion of Depth to Length of Channel**; ($\frac{W}{L}$), **Mobility of Current**; ($\mu_n$), **Capacitance per Square-Unit**; ($C_{ox}$), **Difference of Ground to Source**; $V_{GS}=[V_G-V_S]$**at a difference to Threshold Voltage; represented as the average of $V_{DS}$**; $\frac{V_{DS}}{2}$, multiplied by **the difference of voltage drain and source**; ($V_{DS}$)

$I_D=\frac{W}{L}*\mu_n*C_{ox}(V_{GS}-V_{TN}-\frac{V_{DS}}{2})*V_{DS}$
#### Manipulation of Variables
**Circuit Design Engineers:**
- $\frac{W}{L}$
**Fabrication Parametres**
- $\mu_n*C_{ox}$
**Lab Manipulation**
- $(V_{GS}-V_{TN}-\frac{V_{DS}}{2})*V_{DS}$

### Value of $k_n'$
$k_n'=\mu_nC_{ox}$

### Value of $k_n$

Utilising this simplification, we can take the proportionality that we derived as
$k_n'(\frac{W}{L})(V_{GS}-V_{TN}-\frac{V_{DS}}{2})V_{DS}=$
$k_n(V_{GS}-V_{TN}-\frac{V_{DS}}{2})V_{DS}$

### Drain Current Equation
vErY eAsY tO mEmOrIsE
$I_D=k_n(V_{GS}-V{TN}-\frac{V_{DS}}{2})V_{DS}$

## Relationship of $k_n$ to $V_{DS}, I_{D}$ Proportion
![[Pasted image 20240710101031.png]]
Watch the boundary line; (purple) as the geometry of the resistance channel lessens as the node towards Drain. And soon, equates - and closes off because they are of the same polarity: **Pinch-off**.

### Beyond Pinch-off
![[Pasted image 20240710101550.png]]
The channel's differences remain the same, even if the voltage increases; the channel's proportionality with the proportional pinch-off remains the same. So thusly, it saturates harshly after the pinch-off.
![[Pasted image 20240710101718.png]]

### Drain Current Proportionality Update
![[Pasted image 20240710101848.png]]

### Triode to Saturation
Centre Read boundary line is "Pinch-Off"-Curve separating the two boundaries between Triode and Saturation.
- $V_{DS}\leq V_{GS}-V_{TN}$
- $V_{DS}\geq V_{GS}-V_{TN}$
![[Pasted image 20240710102116.png]]
## Transistor Circuit Analysis
![[Pasted image 20240710102543.png]]
## Transistor Analysis of Triode vs Saturation
![[Pasted image 20240710104312.png]]
![[Pasted image 20240710205411.png]]