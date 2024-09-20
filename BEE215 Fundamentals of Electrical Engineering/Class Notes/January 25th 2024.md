# Preamble
Professor Berger
"It took me 3 hours to keep doing this cause I kept making algebra errors, so I feel your pain if you had problems"
Notes being taken, he was looking to improve node voltage method, so he would put the ground reference near the voltage - so avoid creating a supernode.
#### Notes for reference of sample circuit
Reference node @ C,
Good alternatives to standardised Node B

"Is there an easier way?"
The circuit is equivalent for everything in parallel and everything in series are "swappable" - all circuit elements within' that 'equivalent' may swap places - if 'neighbouring'.

![[Pasted image 20240125132054.png]]![[Pasted image 20240125132159.png]]
#### Combined Example
![[Pasted image 20240125133733.png]]
****Most of the time you can't do this, so you end up using a supermesh***

***For context, creating a situation where references are able to occur over multiple wires as possible.***
- Avoiding using a supernode; prioritisation of a nodal source
- Calculations; algebraically become ease of use
- Moving a node away from the equation
	- Consequentially raises potential around the moved resistor
##### Resistor Review
- Raised potential over a voltage source, is relative to the resistance within' the series, and their series potential
- "Current Laws"

# Mesh Analysis
Nodal analysis is based on KCL
Mesh analysis is similar to Nodal Analysis, in the stead - KVL

***Mesh:*** The voltages around a loop must equal to zero
Synonymous to Nodal Analysis; where in the stead of a node = 0, the entire loop = 0.

* Preamble nonsense: LTSpice uses KCL*
* "Your miles may vary", preferences to nodal analysis over mesh
	* In some cases; mesh is just fater.
	* Identifying characteristics of a faster solving problem

If we have current sources, we have to use the Super Meshes
A mesh is a loop; and a Mesh Current is the current that flows through that loop.
![[Pasted image 20240125133310.png]]

Nodal Analysis; assume the node your working with is the most positive analysis
Mesh Analysis; assume the loop your looking at is the most positive - and you use 'near-side' voltage (the negative side to the positve side).
![[Pasted image 20240125133246.png]]

"***Mesh Analysis & Nodal Analysis are two sides of the same coin***"

***Note that the mesh-current loop that appears in every equation is being written has a positive sign in every term that appears***
__*Do Mesh Currents go in the opposite direction?*__
- Checks for consistency
- Same flowing directions for meshes

***All loops have to be in the same clockwise or counterclockwise directions***
![[Pasted image 20240125134112.png]]
Supermesh; you solve for everything
and then assume an Auxiliary Equation for the inside.

## "How to deal with a dependent source inside a Mesh Analysis"
##### LT-Spice Tangent
"Within' the lore of LTSpice"
- "H" is a Current Dependent Voltage Source
 ![[Pasted image 20240125134510.png]]

Value, and Value2 are the variables; set the value of 'Value' to V2
- LTSpice Manual
- LTSpice User Group
![[Pasted image 20240125135055.png]]
#### Ground Assignment Consideration
***You can assign the ground ANYWHERE***
- Ground describes what is zero volts in the circuit.
- In a pure-math context, math becomes easier depends on ground is
"Electron Microscope Tangent"; 1-million Volts to Ground - Electron Beam is sitting at a 1-million volts.

#### Sample Problem's Solving Strategy; Pg. 19 Example 2 Cont.
1. Identify the loops
	a. Don't take shortcuts. "Just follow the recipe and turn the crank"; Plug & Chug
2. Loop 1
3. Loop 2
4. Solving Loop 1
5. Solving Loop 2
	a. Auxiliary Equation
###### "It's just Algebra", simple, not easy.
#### Power Review
- Power (Watts) = V.I
Consideration to Ohm's Law;
V=IR, allowed substitution for Power equivalents

##### "The best way to learn this stuff"
Just solve a lot of problems.
- Do the same problem in both ways
	- Mesh
	- Nodal
	- Goodlucklmfao

### Be opportunistic
Reduce as many nodes as you can
Reduce as many resistors as you can
Pragmatism

## Next Week @ Superposition
"To solve a much more complex problem more simply"