## Duality
$\delta<=>1$
$\omega_0 <=> 2\pi t$
$e^{jk\omega_0 t}<=>2\pi\delta(\omega-k\omega_0)$

We take the Periodic signal, and remember that 
$\int_{-\infty}^\infty 2\pi\delta(\omega-k\omega_0)e^{j\omega t}d\omega=e^{jk\omega_0t}$

Considering the periodic signal x(t) summation, we can represent as a Fourier Series
$x(t)=\Sigma^{\infty}_{k=-\infty}C_ke^{jk\omega_0t}$

With a respect to a constant
$f^{-1}[f(\omega)]=\frac{1}{2\pi}\int^\infty_{-\infty}f(\omega)e^{j\omega t}d\omega$
= $\frac{1}{2\pi}\delta(\omega-k\omega_0)e^{j\omega t}d\omega$
	Note: $\omega_0=\omega k$
=$\int^{\infty}_{-\infty}\delta(\omega-k\omega_0)e^{jk\omega_0t}d\omega$

## Sampling between the impulses; Shannon's Theorem
Trade-off between resources and sampling accuracy
### Ideal Filter
AM Modulation

## Laplace Transform, Laplace Transform Examples, and Functions
Fourier Transforms are sub-sets of Laplace Transforms
- Using Laplace Transform, differential equations to solve algebraically
- Determine the pole/zero diagrams from the Laplace Transform in determination for the Laplace Transformation
## Definition of Laplace Transformation
*Bi-lateral* $L[x(t)]=X(s)=\int^{\infty}_{\infty}x(t)e^{-st}dt$
We take the complex variable of $s=\sigma+j\omega$

The Inverse Bilateral Laplace Transform of X(s) is:
$x(t)=\frac{1}{2\pi j}\int^{c+j\omega}_{c-j\omega}$
Even if we're not doing-so in this class, this information is relevant to our subject.
Contour integration; Calculus III, the integration of the surface area

The more popular definition:
*Unilateral* $L[x(t)]=X(s)=\int^{\infty}_0x(t)e^{-st}dt$
**Practically:** We're looking to have present time onwards

It could be the same answer, however; it converges from two different sides. We define as it as the "Region of Convergence":
![[Pasted image 20240801153851.png]]

The ROC; from the range of $t_0 < ROC <t_1$
![[Pasted image 20240801153951.png]]
## Example
![[Pasted image 20240801154834.png]]
![[Pasted image 20240801155521.png]]
![[Pasted image 20240801160351.png]]

![[Pasted image 20240801161005.png]]
# Homework Last Problem (3)
We use the integration form if we cannot convert it to Eueler's identity
![[Pasted image 20240801162623.png]]

