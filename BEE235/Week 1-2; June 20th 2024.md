# Matlab Lab 0
https://canvas.uw.edu/files/121727332/download?download_frd=1

Matrix Laboratory
- Computing power dependent

Sample Lab Report
https://canvas.uw.edu/files/121727332/download?download_frd=1

Lab Sign-up Sheets
https://canvas.uw.edu/courses/1737956/pages/lab-sign-up-sheet

Free Matlab Software
https://itconnect.uw.edu/uware/matlab/
https://www.mathworks.com/academia/tah-portal/university-of-washington-31094417.html
# Periodicity of sum of periodic signals
![[Pasted image 20240620142504.png]]
- The period of the new unit is 6
	- It repeats!!!
# Periodicity of Sinusoidal Graphs
![[Pasted image 20240620143557.png]]
# Periodicity Complex Form
![[Pasted image 20240620144619.png]]

# Covered Topics
## Step Function
## Unit Impulse and its Properties
- Mathematically; and real-world application
	- You can compare it to a switch; where a "step" is seen as:
		- Off = 0
		- On = 1
![[Pasted image 20240620145442.png]]

# Rectangular Function
## Translating to a Step Function
### Step-Function Summation: Review from 233 (Impulse)
![[Pasted image 20240620150440.png]]

# Ramp Function
![[Pasted image 20240620150648.png]]
![[Pasted image 20240620150909.png]]
# Time-shifted Delta
![[Pasted image 20240620152436.png]]
# Impulse Function Multiplaction
![[Pasted image 20240620152930.png]]
![[Pasted image 20240620153035.png]]

## Example
![[Pasted image 20240620153400.png]]
## This is when the impulse = 1; because the integration has "Everywhere" become '0'
![[Pasted image 20240620153545.png]]

![[Pasted image 20240620153844.png]]
## Impulse Functions are Symmetrical
![[Pasted image 20240620153919.png]]
## Time Scaling
![[Pasted image 20240620154225.png]]
![[Pasted image 20240620154459.png]]

![[Pasted image 20240620154551.png]]
![[2024_06_20_15_42_28_1.mp3]]
## Strategy of solving
- 1) Evaluating the Step Function @ Impulse
![[Pasted image 20240620155517.png]]
- 2) Solve the step function @ Impulse's $t_o$
![[Pasted image 20240620155528.png]]
- 3) Take evaluated constant as $x(o)$
![[Pasted image 20240620155647.png]]
= 9

# Basic System Properties
## System with & without memory
### System:
operation for which cause-and-effect relations exist
![[Pasted image 20240620160756.png]]
![[Pasted image 20240620160803.png]]
## Memory
Outputs a time $t_o$ depends on the input $x(t)$ for $t>t_o$ or $t<t_o$. Depends on the values of other inputs other than $x(t_o)$, otherwise it is memoryless. It depends on "previous time".
- Capacitor $v(t_o)=\frac{1}{C}\int^{t_0}_-\inf i(t)$
	- It depends on the past values so it has "memory".
## Memoryless
Depends on only "Current" time
- Resistor $v(t_o)=Ri(t_o)$; the voltage depends only on current at time $t_o$
## Invertibility and Inverse System
## Causality
## Linearity
## Time-Invariance
# Stability
