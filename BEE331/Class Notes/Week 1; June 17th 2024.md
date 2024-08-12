# Linear Relation Circuit
"The linear relation between current and voltage"
- Resistor; Ohm's Law
- Capacitor
- Inductor
# Diode Modeling
1) Exponential Model; Best for accuracy
2) Ideal; Fastest however least accurate
3) Constant Voltage Drop (CVD)

# Spice Simulations
Nodal Analysis; majority of spice simulation analysis as a technique.
- We can essentially simulate this through the software.

# Exponential Model
$I_D=I_s(e^{\frac{V_D}{V_T}}-1)$
- $V_D=0$, $I_D=0$
- $V_D=10V_T$
	- $V_T$ (Thermal Voltage)
		- $\simeq25mv$
		- $27^\circ C=300^\circ K$
- $I_D=I_S(e^10-1)$
- $V_D=-10V_T$
	- Hella' small
	- Likely negative -1
- $V_D<0$
	- $I_D\simeq I_S(e^{\frac{V_D}{V_T}}-1)$
	- $\approx -I_s$
# Pos/Neg Relationship
Negative $I_S$ (Reverse Saturation Current)
- Reverse of a diode
- Reverse a saturation
The current conducts from higher to lower; the current still conducts to very small. (Reverse Diode); Reverse-bias
Higher to lower; conducts and exponentially increases (Full Diode); Full-bias
$I_D\simeq-I_S\simeq I_S e^{\frac{V_D}{V_T}}$
# __Our equipment sucks.__
# Node Voltages
$V_a - V_b = 3V = V_{ab}$

# Typical Strategy of calculating Diodes
## Symbolically recognise the circuit
- Design the circuit
- Label the circuit
# Series
Share all the same current
$V_S=I_D*R+V_D$
- Isolate the known variables
- Have the equation equal to the unknown variable
Auxiliary Equation; $I_D=I_S(e^\frac{V_D}{V_T}-1)$
Substituted Equation: $V_S=I_SR(e^\frac{V_D}{V_T}-1)+V_D$
Modified Equation: $\frac{V_S-V_D}{I_SR}+1=e^\frac{V_D}{V_T}$
$ln(\frac{V_S-V_D}{I_SR}+1)=\frac{V_D}{V_T}->V_Tln(\frac{V_S-V_D}{I_SR}+1)=V_D$

# Hypothetical 3 Components in Series
$V_S=3V$
$R=1K$
$V_T=25mV$
$I_S=10^{-12}A$
