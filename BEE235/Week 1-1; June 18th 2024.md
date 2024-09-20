# What is a discrete signal
- On and off; transition between a step function.
# What is a continuous signal
- Transition between an seemingly infinite duration.

# Ultimate Goals of Learning
## Three critical concepts in signal processing:
- Convolution: A mathematical operations
- Fourier Transform: Frequency Analysis
- Laplace Transform: System Analysis

In order of pertinence
- Laplace
- Fourier
- Convolution

Frequency-doman;
- Image recognition; phase transform

Continuous Signal;
- Inputs: Square Signal, of a -1 to 1 x(t)
- Outputs: Resultant Signal; through a LPF (Low Pass Filter); y(t)
![[Pasted image 20240618142516.png]]
It "crispens" the edges in a contrast
# Microphone Functions
- Mechanical; Analog function
- Electrical coorelation to voltage to analog data

# Signal
- Grating colour sensor coorelation to voltage changes

# System
- Modifies; extracts and digitise the analog data (ADC) Mechanical Data.

# Producing things from Continuous Time to Discrete Time
![[Pasted image 20240618143706.png]]
Analog Data; ADC to Step-function

$S^\inf_{t=0}in(wt)$
$\Sigma^\inf_{n=1}Sin(2\pi nt)$

# Convolution Operations
- Time-reversal
	- $y(t)=x(-t); x(t)$
![[Pasted image 20240618144224.png]]
- Time-scaling
	- $y(t)=x(\alpha t)$

Compressing $\alpha >1$
![[Pasted image 20240618144518.png]]

Expanding $\alpha < 1$
![[Pasted image 20240618144815.png]]

# in-class exercises
![[Pasted image 20240618145116.png]]
- It's essentially substitution
- Time-shifting $y(t)=x(t-t_o)$
![[Pasted image 20240618145614.png]]
![[Pasted image 20240618150001.png]]
