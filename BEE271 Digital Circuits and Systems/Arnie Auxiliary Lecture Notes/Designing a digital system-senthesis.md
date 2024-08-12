- Synthesis is the process of beginning with a description of the desired functional behaviour and then generating a circuit that realises that behaviour
![[Pasted image 20240404153521.png]]
*Correct*, but in terms of engineering, this isn't ideal
In boolean algebra, we can reduce it as
- $\bar{x_1}\bar{x_2}+\bar{x_1}x_2=\bar{x_1}(\bar{x_2}+x_2)=x_1$
- 
### Arnie Lecture
We move from a truth-table into boolean equation, into simplification
- There are ways to do this is 
	- Switching between positive logic to negative logic
	- Karnaugh-Maps
## Cost-realisation
The total number of gates plus the total number of gate inuputs
![[Pasted image 20240404153708.png]]
Cost of
6(gates) + 11(inputs) = 17
Propagation delay of 3-gates

![[Pasted image 20240404153800.png]]
Cost of
2(gates) + 3(inputs) = 5
Propagation delay of 1 

# Bubble gum factory Example
![[Pasted image 20240404154013.png]]
![[Pasted image 20240404154107.png]]

![[Pasted image 20240404154225.png]]
# Min-terms
![[Pasted image 20240404154305.png]]
## sample
![[Pasted image 20240404154408.png]]
# PAL: Programmable Array Logic
An integrated circuit you can program

And is designed to give you two sum-of-product terms for 4 possible inputs.
## Generic Array Logic: GALs

--
![[Pasted image 20240404154852.png]]
# Product of Sums
*In the stead of excluding terms of f=0, we instead exclude terms of f=1 using Maxterms*
![[Pasted image 20240404154958.png]]
![[Pasted image 20240404155218.png]]
# Cookbook Approaches
- Consider the truth table
- POS considers MAXTERMS f=0
- If any one of MAXTERMs = 0, then f = 0
	- e.g. M_0, M_2, M_3, M_7
		- f = 0
- MAXTERM form of (A+B+C)
- At least zero in at least one MAXTERM
	- $0 = x_n$
	- $1=\bar{x_n}$
- Thus $f = M_0*M_2*M_3*M_7$
	- $f=(x_1+x_2+x_3)(x_1+\bar{x_2}+x_3)(x_1+\bar{x_2}+\bar{x_3})(\bar{x_1}+\bar{x_2}+\bar{x_3})$

Use the methodology while realising functions of only when costs reduce.
	POS & SOP aren't always equivalent in cost.
*Product-of-Sum isn't always commonly used, however, it is still used in some cases if they produce an equivalent cost*

**Using the terms with the least involved combination of terms**

![[Pasted image 20240404160226.png]]
In a circuit like this, it's a $2^3$ truth table with 8 outputs
In this case, it would be Product-Of-Sum's ideal case.