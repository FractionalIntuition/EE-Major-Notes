- When we do the convolution function with a signal impulse, we have the signal that is the *same signal*.
	- Associative Property
	- ![[Pasted image 20240709144259.png]]
	- Distributive Property
	- ![[Pasted image 20240709144454.png]]
Every signal is an arbitrary combination of the following signal transformations and so it is very powerful.
Example Slide @ Impulse Response for an interconnection of any system.
![[Pasted image 20240709144035.png]]
# Review
Causal
![[Pasted image 20240709145014.png]]
Stability of an LTI Systems
- BIBO
	- In order for a value to y(t) to be equal to the bounded region of $G<\inf$
	- ![[Pasted image 20240709144944.png]]
- NOT STABLE
- ![[Pasted image 20240709144929.png]]
# BIBO
## Bounded Input, Bounded Output
![[Pasted image 20240709145509.png]]
Is stable?
![[Pasted image 20240709145718.png]]
No!
![[Pasted image 20240709150328.png]]

![[Pasted image 20240709150317.png]]
# Fourier Series
## a foundation for the Fourier Transformation
Time Domain to Frequency Domain is a Fourier Transformation. Sin and Cosine function to the series.
### Periodic Signals
![[Pasted image 20240709151300.png]]
![[Pasted image 20240709151347.png]]
We take cosinal terms that are synthesisesd to the replications are the signals being stacked together until they are able to be added together to simulate a wave form *almost close enough* to a square wave form.

This is what Fourier Hypothesised; that we compound the signals together, they would resemble *to something similar to a square waveform*.

Each one of these half-divisions of the signals is termed as a "Harmonic".
![[Pasted image 20240709151519.png]]

### Harmonics
https://en.wikipedia.org/wiki/Harmonic#:~:text=In%20physics%2C%20acoustics%2C%20and%20telecommunications,are%20known%20as%20higher%20harmonics.

*Takeaway; *
- Harmonics
- Fourier Transform
	- Fourier Series
	- Laplace
	- Monge
	- Lagrange

Differential Equations found in a daily life; the daily life solutions become the input to the system.
$\Sigma^\infty_{k=-\infty}c_ke^{jk\omega_0t}$
Periodic Signal is a time signal, with the involvement of the time.
- $\omega_0=2\pi f_0=\frac{1}{T_0}$
	- $x(t)=x(t+T_0)$
- $k=$ Harmonic approximation; per harmonic; so it's 1, 10k, 20k, 40k
	- $k=0$ Give DC (zero frequency) signal
	- $k=1$ Signal; harmonic of 1, is the signal itself
	- $k\geq2$ The signal is a harmonic.
	- **$k$ must be a natural number**
- $c=$
$c_0=\frac{a_0}{2}$
$c_1=\frac{1}{2}(a_k-jb_k)$
$c_{=k}=\frac{1}{2}(a_k+jb_k)$

![[Pasted image 20240709154411.png]]
![[Pasted image 20240709160321.png]]
# Differential Equations
