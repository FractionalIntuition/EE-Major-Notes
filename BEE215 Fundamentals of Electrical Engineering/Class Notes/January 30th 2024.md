# Exam information
## Saturday Morning Room 205; Review
## All units covered until this Thursday
- Thevenin & Norton is the latest coverage
	- Simulate a giant complex circuit by using a simple circuit
	- Most practical use in Electrical Engineering
		- Most often used
- Review midterm worksheet being given this Thursday
- Thursday's lecture; simple review day
	- Source Transformation Coverage
- **Tuesday will mirror this, for the upcoming Exam Thursday**
	- "Hopefully this would give enough practise to hone your skills"

# Superposition
## A physics principle & quantum mechanics
### Preamble
A particle can exist in multiple space at the same time; "Schrondinger's Cat" - dead and alive at the same time. (Paradox)

### Schrodinger's Cat
A radiation source, randomly can emit radiation; and the radiation detector drops a hammer and breaks a vial of cyanide gas. The cat is in the box and... to the outside observer, depending on when you look in the box is either alive or dead - the cat's state of life is randomness is determined by the time at which you looked into the box.

### Superposition
**A circuit simplifying method, that turns a more complicated circuit easier to analyse**
- "In my personal opinion, takes longer"
	- You solve 2 or 3 separate problems where you can just solve only 1
- "It's kinda' nice when you can clearly break down the circuit simply"
- 
**Learning Objective**
- Solving mutli-source circuit
- When to use it

**Overview**
- You take a circuit with severeal independent voltage or current sources
- In order to characterise the circuit (solve for current or voltage values),
- 1) Eliminate all but one of the sources
- 2) Repeat the solution for each source
- 3) Add the separate solutions together
Hypothetical psuedopure-math
$\sum S_n = S_{V1} + S_{I1}  + S_{V2}$

Essentially for every source, you solve the circuit one more time for every source available
$\sum S_n = n = Solve\space count$

**Source Transformation**
Voltage Sources become closed-branches
![[Pasted image 20240130133351.png]]

Current Sources become open-branches
![[Pasted image 20240130133607.png]]

**When zeroing out sources in the circuit, realise we have simple voltage and current dividers**
- Current source; Voltage Divider
- Voltage source; Current Divider
	- Mind the polarity

**Summate all the separate source-specified equations**
$\sum R_n = R_{n_1} + R_{n_2} +\space ...\space + R_{n_n}$

## If you don't get the answer you're expecting in the textbook
### "Just throw it into LTSpice"
- Put it into LTSpice first
- Get the answers first
- Then solve working towards the answer to determine where your error is
*Simulations in general*

*Experienced engineers don't bother redrawing it, they just put their thumb over the source and get to the solutions.*
*A real circuit professional can write the equations for **i** directly*

**Remember that superposition only works with current or voltage, not power**
We're still able to do the power calculation, but you need to solve the entire circuit first.

### Rules for dependent sources
- You cannot zero dependent sources - you have to leave them in the circuit.
- It's still a problem dealing with both independent and dependent sources
![[Pasted image 20240130134815.png]]

### Superposition places a premium on
- Opportunistic use of KCL, KVL, Ohm's Law, Series, and Parallel combinations - as well as current and voltage dividers
- Visualising what the circuit would be if sources were removed
- Recognising circuit structures like current and voltage dividers
- Works for linear circuits, doesn't work for power
- To use it, is to "Zero the sources" - and respective above

## Next Thursday
**Equivalent Circuits**
Which will complete the course