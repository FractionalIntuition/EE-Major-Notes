
A random variable is a variable whose numeric value is determined by the outcome of a probability experiment e.g. x,y,z,...

Demo 'Y' on and friends went to a spring festival. One game of a carnival is a coin-toss challenge you get a chance to flip 3 fair coins.
- If all coins are the same; {HHH, TTT}
	- You win $3, otherwise you get nothing

Outcomes | HHH | HHT | HTH | THH | TTH |THT | HTT | TTT |
Probability|    $\frac{1}{8}$   |    $\frac{1}{8}$   |    $\frac{1}{8}$   |    $\frac{1}{8}$   |    $\frac{1}{8}$   |    $\frac{1}{8}$   |    $\frac{1}{8}$   |
	x       |   3     |    2    |   2   |    2    |    1  |   1   |   1   |   0   |

Next: Discrete Probability Distribution

	x       |   0  |   1    |   2   |    3  |
	P(X)=x) | 1/8  |  3/8   |  3/8  |  1/8  |
- $P(x=0)=\frac{1}{8}$
- $P(x=1) = \frac{3}{8}$
- $P(x=2)=\frac{3}{8}$
- $P(x=3)=\frac{1}{8}$

A probability distribution is a table of discrete or a formula that gives the probability for every value of a random variable {X}.

#### Given a random variable {X}, $P(x) = P(X=x)$
The name of the value is $pmf$; Probability Mass Function.
- They'll give you a table and ask you to find the probability to outcomes equations $P(X=x) = \frac{a}{b}$
$F(x)=P(X=x)$, familiar means it's amongst frequency tables.
![[Pasted image 20240411112906.png]]
$P(2\leq x \leq 3)$
P(X of most 2)
= P(X = 2) + P(X=1) + P(X=0)
OR
1-P(X=3)
= 1-1/R = $\frac{7}{8}$

The expected value of a discrete r.v. (Random Variable); {X} is equal to the mean of probability distributions and given by
E(x) = $\mu$ = $x_i * P_{x_i} =^{or} \Sigma x_i * P(X=x_i)$
- i stands for "index"

## Example
Back to Demo; (Coin-toss Challenge)
- You win $3 or walk away with nothing
- {HHH, TTT} or {Everything else - HHH,TTT}
Let W = Discrete R.V. with Values 3 or 0
Probability Distribution of W is given
![[Pasted image 20240411112934.png]]
$E(w) = \Sigma w*P(W=w) = (3)(\frac{1}{4})+(0)(\frac{3}{4})=\frac{3}{4}=\$0.75$
If you were to play the game an absurdly large arbitrary number of times, you would expect on average gain of $0.75 each game you play.

### How can we find the variance and deviation?
Variance and Standard Deviation of Discrete r.v. {X} is given by
$\sigma^2 = \Sigma _{All_{x_i}} (x_i - \mu)^2*P(x_i)$ <- Var(x)
$E(X^2_i)-\mu^2$; Short.

$\sigma = \sqrt{\Sigma (x_i - \mu)^2 P(x_i)}$

## Example 2 Find the variance and the standard deviation of W on E(1)

![[Pasted image 20240411114506.png]]
$\sigma^2 = 1.6875$
$\sigma = 1.2990$

## A binomial distribution is a special probability distribution with a fixed number of independent trials  (n) where each trial has only two possible outcomes and one these outcomes 1's counted as success (with% P)
A binomial distribution (for a discrete random variable (r.v.) {X}) has the following characteristics:
- Experiment consists of fixed # of tirals (n)
- Each trial is independent of the others
- For each trial, there are two possible outcomes
- For a trial P(Success) = P, P(Failure = 1-P
- The binomial r.v. {X} counts the # of success
- For a binomial distribution {X$\cong$B(n,P)}
## Example: Consider the experiment of tossing a fair coin 58 times.
Kx X: # of Heads
- a) Is X a Binomial r.v.?
	- Yes, X~B (58=n, 0.5=O)
- b) How many times do you expect to get a head.
	- $\mu = nP=(58)(0.5)=29$
- c) Calculate the Standard Deviation & what does it tell us?
	- $\sigma^2 = nP(1-P)$
	- $\sigma = \sqrt{nP(1-P)} = \sqrt{(58)(0.5)(0.5)} = 3.8$

The pmf for a Binomial Probability Distribution for r.v.{X}
![[Pasted image 20240411121657.png]]
## Example 2: 
![[Pasted image 20240411122405.png]]
![[Pasted image 20240411124027.png]]
# Poisson Distribution
The Poisson distr. of a r.v. {X} Count the # of successes in a given interval such as part of time.
Characteristics 
- Each success must be independent from any other successes
- Count # of successes in a given interval
- Mean # of successes in a given interval must remain constant $\lambda$
	- X~Pass.($\lambda$)
- The mean and variance of x $\mu = \sigma^2 = \lambda$
- Part of $\mu X = P(x) = P(X=x) = \frac{e^{-\lambda}*\lambda^x}{x*1}$
	- $x = 0,1,2,...,n$
## Example 3.5 (supposedly)
Suppose a length of copper wiring averages one defect every 200 feet. What is the probability that 300ft  sketch will have no defect?
Is it Poisson? Yes,
- Find $\lambda = 1.5$
	- 200ft -> 1 defect
	- 300ft -> 1.5 defects
P(X=0) = $\frac{e^{1.5}*1.5^0}{0!} = e^{-1.5}= 0.2231 = 23.31\%$
$P(X\leq 2) = P(x=0) + P(x=1) + P(2)$
- = Poisson $Cdf (\lambda,x) = 0.808$