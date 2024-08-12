## Typically across a diode equation; Ideal
1) $V_S=I_D*R_S+V_D$
2) $I_D=I_S(e^{\frac{V_D}{V_T}}-1)$
We need to satisfy the variables for both equations and try to solve it symbolically then numerically as going forward.

Similarly; to satisfy both equations; we approach the graphical method utilising the $I_D$ equation, and the $V_s$ equation graphically; pictographically.

$V_S$; Load Line, behaviour of the circuit in perspective of an ideal diode. Essentially a linear circuit.
- The characteristics of the load line is linear, declining; $I_D=\frac{V_S-V_D}{R_S}$
$I_D$; Exponential line; are the exponential components include the current

The "load" in a "load-line", is described by the load across the diode curve; the exponential curve. Where we analyse the the behaviours of the circuit without full context.

Of a **linear-circuit;** the best-practise of a technique to find our $V_{out}$; equivalent to $V_D$.

![[Pasted image 20240626084856.png]]

# The load-line
We;
- 1) Find $V_D=0$
- 2) When $I_D=0$
![[Pasted image 20240626085911.png]]
## Load-line review
*see attached*
![[Pasted image 20240626091019.png]]
# Circuit Analysis of 2 Diodes
*See attached*
![[Pasted image 20240626091411.png]]
## For the above circuit, we'll be using either
- Ideal Diode Model
- CBT Diode Model

## Ideal Method
**Even though there's two diodes; the procedure is the same - you just have to make *two* presumptions**
We have a total of 4 possibilities of diode combos; combination. $2^2$; off of perception.
![[Pasted image 20240626091925.png]]

*Side note: Start using ground symbol and not a black-arrow to signify ground (reference node)*

# CVD Diode
## How to know the "activation" value of the diode
Read the schematic sheet
# Diode information
*Typically found in the schematic for the given information*
## Power Rating
The limitation of what the diode can handle; before bursting into a beautiful fireball
## Activation Threshhold
The minimum threshhold before it "activates".