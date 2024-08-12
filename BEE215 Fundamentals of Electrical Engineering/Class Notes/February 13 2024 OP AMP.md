An OP-Amp is an voltage dependent source

Thousands of different types of OP AMPs out there.

They're complex devices, with many of the components of

The gain is nearly infinite - and the gain when given a metric
- A little bit of voltage can increase magnitudes in output

The task of choosing the correct OPAMP is part of the engineering job, the ideal relationship breaks down.

We have to concern ourselves when the ideal breaks down.

Use the tools applied, the OPAMP circuits are real circuits you'll be using in real life....

### Intention
How to solve them
When they break down
When they saturate
How we'll select them
How we'll analyze a non-ideal op-amp

### No history questions on the exam

The op-amp, it has a plus ans a minus connection.
The connections are non-inverting inputs and inverting inputs, respectively.

In an ideal case, the voltage is infinity x v-out ![[Pasted image 20240213140406.png]]

## Two rules
- V1 and V2; two input voltages are always equal
- No current goes into the Op-Amp

From that, everything else flows.

8-pin, plastic packages

Inverting and non-inverting is relative to the output
## Follower Circuit
![[Pasted image 20240213141009.png]]
Voltage drop is 0
$V_2$ is equal to $V_s$
They have to be the same.

The output is connected by the voltage input. The output is equal to Vs.

Any kind of circuit behind the follow Op-Amp is Thevenin's Circuit.

That will give out to the output behind it. And when we get rid of the OpAmp, it will rid of the zero voltage drop. There's no Thevenin Resistance in the OpAmp so its an ideal source.

They are also synonymously regarded as 'Buffer' OpAmps.

You can take the circuit and boost the current. And with the buffer follower OpAmp, it removes the equivalents.

## Saturation
If we actually built one of these Voltage Followers, and varied the V2. The output may stop tracking the input.
It looks like an ideal source until it isn't, and the current output cannot be supplied anymore.
It is saturating when it moves out of the linear region.

$|V_o|<= v_{set}$
$|i_o| <= i_{set}$

#### Sample problem:
Suppose we have a saturation voltage source, without saturation, the biggest load we can put on there is 5k$\Omega$

#### Slew rate
741 should not be an OpAmp we use today
$\frac{dv_o}{dt}$, we're looking at DC circuits, right now AC circuits.

![[Pasted image 20240213142745.png]]
![[Pasted image 20240213143333.png]]