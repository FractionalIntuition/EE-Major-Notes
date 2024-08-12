An ALU is an array of combinational logic. It has logical inputs: operands, and commands on what to do with those operands. LOgical outputs are the results, adn status bits describing those results.
https://www.youtube.com/watch?v=gTg33Ox1SCk&list=PLsHOxmMgAiQwL8X_-0KjQLmtKUB67nd3m&index=5

# Basic Architecture
- Simple
- Each function is carried out by a particular circuit
- The inputs are fed into the circuit
- Which circuits output is fed to the single **ALU (Arithmetic Logic Unit)** output is determined by a series of **multiplexers (MuX)**
- The **control bits** of the ALU are used to control the various Multiplexers and route the signals around
- The operations can be split into **logical** or **arithmetic** unis
	- https://sites.google.com/site/embeddedmonologue/home/c-programming/logic-and-arithmetic-shift-and-divide-by-2
	- https://gcc.gnu.org/legacy-ml/gcc/2000-04/msg00152.html

## Top-level Design
Top-Level Design; same logic as programming, High-Level or Low-Level.
Briefly describing all platforms, systems, processes, and any important changes to the design.
![[Pasted image 20240203203047.png]]
### Arithmetic Unit; Operations
- Arithmetic operations are typically limited to **addition** and **subtraction**
- The hardware to do these operations is easy to design and implement
- (Relevant) In reality, most ALU's will implement a **carry look-ahead** adder rather than a **ripple carry** adder as they can carry the operation out quicker
	- For this lab, we're utilising a **ripple carry** adder for our circuit for **binary addition**
![[Pasted image 20240203222012.png]]
- **Binary Subtraction**
	- Can actually be carried out by the binary adder
		- $y= A-B = A+(-B)$
			- **B is negative, and can be represented in using a 2's complement**
			- $-B=\bar{B}+1$
			- $y = A+\bar{B}+1$
		- 
- Some microprocessors may also have hardware **multipliers**
	- The hardware of a multiplier is more complex in a circuit overall and won't be covered in this lab or circuit.

## DE-10 Implementation
https://scalable.uni-jena.de/opt/ehp/chapters/assignment_alu.html#designing-a-basic-alu
