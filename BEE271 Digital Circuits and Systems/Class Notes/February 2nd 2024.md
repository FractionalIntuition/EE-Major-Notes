## Textbook Chapters
2.1~2.14
2.17
3.1~3.3 (except 3.3.4)
3.5.1, 3.5.2
4.1~4.3 (except 4.2.1 & 4.3.2)

## Multiplexers
### Should you be able to use Multiplexers for 'every' truth-table
No.

## Decoders
n-to-$2^{n}$
Only one output is selected.

| A | B | $Y_o$ | $Y_1$ | $Y_2$ | $Y_3$ |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 0 | 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 0 | 0 |
| 1 | 0 | 0 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 | 1 | 1 |
![[Pasted image 20240201085405.png]]
Why do we need to use multiplexers, decoders, and encoders?

Presuming the Enabler **EN** does not have any input, then it will remain off.
Inputs are relevant to their position as the decoder will allow.

| $Y_0$ | $Y_1$ | $Y_2$ | $Y_3$ | A | B |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 0 | 0 | 1 |
| 0 | 0 | 1 | 0 | 1 | 0 |
| 0 | 0 | 1 | 1 | 1 | 1 |
Essentially an inverse of an encoder. Decoder states.

## NOT COVERED ON MIDTERM
Flip-flops, "storage element of representing a 'state' in a circuit"
Combinational Circuits are based on conditionals; input and output

Sequential Circuits are based on storage elements, which describe time-depdennt logics.

If the input of an &&-gate, the input of a single input being 0 would dignify it as false

If the input of an ||-gate is logically dependent on only 1 of the variables to be true to be considered a true-state.

The glitches in real life occur when logic gates of multiple circuits create an unwanted, delayed, or misguided input.

The input of a sequential logic gate having a guided autopilot would be a given input such as a wire into a '1'.
A delayed input occurs when a pilot is in charge - for the sample - reducing a 'not' gate from the circuit, we would control the input and the output at the same time.
![[Pasted image 20240201092410.png]]
![[Pasted image 20240201092431.png]]
The clocks are represented as purple boxes independently syncing everything together.
The signals are adjusted correctly to be over a period of time - adjusting each pulse to a period.

Period: $T = \frac{1}{F}$
We can guarantee to delay the proceeding pulses to sync with the previous pulses.
The sync of the high-speed clock sets up the complex logic gate circuit to be eliminating glitches.

The example would be a single-state the Washing Machine, as one state of a washing machine can only maintain one state.
- D-Flipflop
- D-Latch

## Active-High Latch
![[Pasted image 20240201092940.png]]
The output depends on the values of whatever the *other* gate's output is.

![[Pasted image 20240201093349.png]]

| S | R | $Q_a$ | $Q_b$ |
| ---- | ---- | ---- | ---- |
| 0 | 0 | 0/1 | 0/1 |
| 0 | 1 | 0 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |
The first-case of S = 0, R = 0, then the state is undefined.
If one of the logic-gates are faster than the other one, then we're looking at whatever is the 'first-value'.

### AND S-R LATCH Active-Low Latch

![[Pasted image 20240201094014.png]]

| S | R | $Q_a$ | $Q_b$ |
| ---- | ---- | ---- | ---- |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 0 | 1 |
| 1 | 1 | 1/0 | 0/1 |

We can fix the Gated SR Latch as a fixed-state circuit.
![[Pasted image 20240201094618.png]]
This circuit depends on what its previous state was.

| CLK | S | R | Q(t+1) |
| ---- | ---- | ---- | ---- |
| 0 | 0 | 0 | Q |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | X |
For the last-cell, it's a hold-state, so we set it up as a "X"; representative as a 'don't care'

## Homework Problem Coverage
### 4.
![[Pasted image 20240201100054.png]]
## 5.
![[Pasted image 20240201101908.png]]

### On-board example 4
![[Pasted image 20240201100918.png]]
