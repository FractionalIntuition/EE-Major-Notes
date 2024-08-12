$E(T_n) = E(X_1+X_2+...+X_n)=E(X_n) + E(X_2) + ... + E(X_n) = n\mu$
$V(T_n) = V(X_1 + X_2 + ... X_n) = V(X_1) + V(X_2) + ... + V(X_n) =$
- $= \sigma^2_1+\sigma^2_2+...+\sigma^2_n = n\sigma^2$
$\sigma_{T_n} = \sqrt{n*\sigma^2} = \sqrt{n}*\sigma$

|          |
| -------- |
| (っ˘ω˘ς ) |
Also,
1. $E(\bar{x}) = E(\frac{X_1+X_2+...+X_n}{n})=\frac{1}{n}\Sigma{i=1}^nX_i$
2. $V(\bar{x})=V(\frac{X_1+X_2+...+X_n}{n})=(independent)=\frac{1}{n^2}\Sigma^n_{i=1}V(X_i)$
3. $\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{n}}$

**Question: What is the shape of the distribution of $T_n$=$\Sigma^n_i=1$ and the sample mean $\frac{\Sigma^n_{i=1}}{n}$**
1)  If $\bar{x}$ is normally distributed with $\mu_{\bar{x}}=\mu$ and $\sigma_{\bar{x}} = \sigma$

2) If $x_i$; i=1,2,3,...,n, are not normally distributed and sample size n is large enough (n>30), then $\bar{x}$ is approximately normal with $\mu_{\bar{x}}=\mu$, $\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{n}}$

**Question: The time taken by randomly selected for a mortgage to fill out a certain form has a normal distribution with mean value 10 minutes; and standard deviation of 2 minutes.**
1) *What's the probability that an applicant will fill the form in at most 11 minutes?*
	- $X~N(\mu,2)=X~N(10,2)$
	- $P(X\leq 11)=0.69146=69.146\%$
![[Pasted image 20240502113845.png]]
2) *If 5 individuals fill out a form on a day, what is the probability that their average time to fill the form is at most 11 minutes?*
	- $P(\bar{X}\leq 11)$
	- $\sigma_{\bar{x}}=\sqrt{2}{\sqrt{5}}=\bar{x}\approx.8944$
![[Pasted image 20240502114054.png]]
# Presumably 5.5; The distribution of linear combination
**The __Sample Mean__ $\bar{x}$ and Sample Total T are special cases r.v. is that shows up in the applications** (☆ω☆)
Given the r.v. $x_1,x_2,...,x_n$ and $a_1,a_2,...,a_n$ real numbers. $\mu_i$, $\sigma_i$ are the mean and standard deviation of $x_i$ for $i=1,2,...n$
- "The linear combination of the mean is the linear combination of their means"
1) $Y=a_1x_1+a_2x_2+...+x_n$
	- Linear combination of $x_i; i=1,2,...n$
2) $E(a_1x_1+a_2x_2+...+a_nx_n)=a_1E(X_1)+a_2E(X_2)+...+a_nE(X_n)$
	- $=a_1\mu_1+a_2\mu_2+...+a_n\mu_n$
3) If $X_1,X_2,...,X_n$ are independent than $V(a_1x_1+a_2x_2+...+a_nx_n)=$
	- $=a_1^2V(X_1)+a_2^2V(X_2)+...+a_n^2V(X_n)$
	- $a_1^2\sigma_1^2+a_2^2\sigma_2^2+...+a_n^2\sigma_n^2$
	- and,
		- $\sigma_{(a_1x_1+a_2x_2+...+a_nx_n)} =$
		- $=\sqrt{a_1^2\sigma_1^2+a_2^2\sigma_2^2+...+a_n^2\sigma_n^2}$
4) For any $x_1,x_2,...,x_n$ (Not necessarily independent)
	- $V(Y) = V(a_1x_1+a_2x_2+...+x_n) = \Sigma^n_{i=1}\Sigma^n_{j=1}a_ia_j*Cov(x_i,x_j)$
	- Cov = "Covariance"
		- **For independence**
			- $Cov(x_i,x_j)=0$; when $i\neq j$
			- $Cov(x_i,x_j)=\sigma_i^2$; when $i=j$
"You start with i = 1, then you begin to measure the calculations when the variable 'j' is 'running'.
![[Pasted image 20240502120103.png]]

**Determining Dependency**
When the covariance is greater than zero, they are dependent. 
Just because the covariance is 0, doesn't mean they are independent
- If covariance is not even mentioned, they are independent. *Assume that*. 
#### Note: (referencing to above)
**In earlier work, (3) is a spread of ($) since if $x_1,x_2,...,x_n$ are __independent__ then $Cov(x_i,x_j)=0$** for $i \neq j$

For clarification
The terminology of Covariance is only used when the X's are different.

If there is a match, we just go into the "Sigma" and square that value as the variance.

# 6.1
Chapter 6 is basically just confirming the idea of Week 1 stuff, the population; within' the sample, when we get the mean

We can use that as an estimate, for the same concept for the population

And in the section when we read through, we find out the mean, the proportion, the standard deviation - they are unbiased estimators. That means, we could use them without conflict; no bias.




























# Super shy, super shy, but wait a minute while I make you mine, make you mine ( ´ ∀ `)ノ～ ♡
![[Pasted image 20240502120136.png]]