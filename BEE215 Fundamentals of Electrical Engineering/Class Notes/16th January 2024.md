#### Quiz Comprehension Review
- Do problems in the back of the book
##### Expectations
- KCL
- KVL
- Able to identify
	- Nodes
	- Loops
	- Wires
- Resistors in
	- Parallel
	- Series
"This is foundation of circuit analysis, this is how the simulators do it"
"This isn't theory, this is done all the time. And will be simulated in LTSpice"
## Node
Points of connection in a circuit

**Definition of a node:**
*Articulated by Professor*
"A node is just a point where circuit elements come together, you can store charge in there"

"The sum of currents flowing into a node is zero"
Current enters the node, the sum of all currents flowing out of a node equate to zero.

KCL Mathematical relationship in a node
![[Pasted image 20240116134059.png]]
**Recognizing the figure above**, the summation of all current entering the node is equivalent to the summation of all current leaving the node.

**Understanding Sign-conventions**
*Without realising the actual values of the current first*
The arrow coming out of a node, you assign the current a negative term.
The arrow entering a node, you assign the current a positive term.

*We formulate the equation based on which way the arrow is going*
**Thinking that the sum of i3 is the sum of what flows in minus what flows out.**

### Proof in LTSpice
![[Pasted image 20240116134233.png]]
**Realizing the figure above, the sum of the current flow is balanced so there is no voltage across the resistor**
Like a voltage source can supply and hold the source, the current source can hold a current and adapt any voltage across it.

*Both nodes are the bottom and the top of the circuit are zero, since the sum is balanced*
- Ideal source
- Adjusts output to what it has to be
- Current is circulating
## Wires
Connections between elements
- Ideal wires have zero resistance, noting that real wires have some resistance
	- Based on a cross-sectional, resistivity, and conductivity
	- "This is why during Christmas we have house fires, cause people just plug a bunch of things into a wall-socket"
- Are short circuits
 ![[Pasted image 20240116133420.png]]
"Hop-over"

*Get into a good habit of drawing your circuits in a consistent manner*
## Loops
### The sum of a voltage around a loop is zero
# Kirchhoff's Voltage Law & Current Law
## KVL
### Kircchoff's Voltage Law relies on loops
#### Strategy for writing an equation
1. Pick a starting point
2. Start walking in either a clockwise or counterclockwise direction
3. Decide either you will take the near-side or the far-side of a circuit element
4. Keep going 
![[Pasted image 20240116135210.png]]
Ways of solving this circuit
**1. Clockwise and far-side:**
**2.**

Finding the missing voltage in the loop is to find the summation of a loop, and realising it equals to **zero**.
![[Pasted image 20240116135443.png]]
## KCL
The simulations use KCL

### Resistor
Source flowing over two resistors is a __series resistor__
![[Pasted image 20240116135637.png]]
1. Simplify the circuits by replacing the two or more resistors
2. Knowing
Once you find the voltage across the equivalent resistor, you won't be able to find the voltage across its components.
**The resistor in series add!**

## Voltage Dividers
*Sample Equation:* Vs = i(R1 + R2)

**1.** Solve for 'i' >> i = Vs/(R1 + R2)
**2.** By Ohm's Law v1 = iR1

*Therefore*

*V1 = Vs.(R1/(R1+R2))*
*V2 = Vs.(R2/(R1+R2))*

In actuality, the
***"This is an equation you should just know"***
