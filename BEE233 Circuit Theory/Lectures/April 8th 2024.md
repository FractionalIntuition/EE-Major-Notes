# Preface
## Inductor
10mH = L
$X_L = j\omega l = j2\pi*f*L\Omega$
## Capacitor
$10\mu F$ = C
$X_C=\frac{-j}{\omega C}=\frac{-j}{2\pi*f*c}\angle(-90^\circ)$
![[Pasted image 20240408153447.png]]
# KCL, KVL, NODAL ANALYSIS
## KVL
![[Pasted image 20240408153811.png]]
$\Sigma V_{rises} = \Sigma V_{drops}$
Law in KVL: $\Sigma V_n = 0$
$\Sigma V_{rises} + \Sigma V_{drops} = 0$
### Near-side
![[Pasted image 20240408154021.png]]
### Far-side
![[Pasted image 20240408154152.png]]
### Ohm's Law
![[Pasted image 20240408154258.png]]
![[Pasted image 20240408154452.png]]
### Voltage Divider
![[Pasted image 20240408154646.png]]
![[Pasted image 20240408154815.png]]
![[Pasted image 20240408160949.png]]
#### Finding Current w/out Current Division?
$I_{R_{11}} = \frac{V_6}{R_{11}}$
$I_{R_T = \frac{V_4}{R_T}}$
$I_{R_3} = \frac{V_2 - V_3}{R_3}$

### "Roadside Traffic" analogy
- The control for how much roadside traffic occurs; the "width" of the road is Resistance or Impedance
### Current Law
![[Pasted image 20240408161801.png]]
![[Pasted image 20240408163445.png]]
### Domain Change Examples:
#### KCL, KVL
![[Pasted image 20240408165445.png]]
![[Pasted image 20240408170220.png]]
# Nodal Analysis
### Basere Technique
Don't even care about current flow; just assume leaving the node
- Identify the Nodes
 ![[Pasted image 20240408170811.png]]
 - Identify the branches
![[Pasted image 20240408171045.png]]
- Remove branch labels when we finish
![[Pasted image 20240408171158.png]]
# Example
![[Pasted image 20240408171457.png]]
- Can't use Voltage Division
- Can't use Current Division
- Can use Nodal Analysis & Mesh Analysis
![[Pasted image 20240408171933.png]]
- Set up equations + auxiliary
- Apply KCL @ V1 node i-
![[Pasted image 20240408172216.png]]
- Now, plug in the numbers
- And remove the assumptions when we're done
![[Pasted image 20240408172424.png]]
![[Pasted image 20240408172443.png]]
- Apply KCL @ Node $V_2$
![[Pasted image 20240408172821.png]]
- Remember to erase assumptions
![[Pasted image 20240408172846.png]]
- Matrix
![[Pasted image 20240408173145.png]]
- Solve for $i_o$
![[Pasted image 20240408173319.png]]
