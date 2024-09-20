# Sequential Circuits
## Synchronous
- The entire system is ran under a single clock signal, used in the operation of all flip-flops
## Asynchronous
- No clock is used
	- All flip-flops and mechanisms are running independently of each other (asynch) Remember your Discord bot knowledge, Jason
### Sequential Circuits; Finite State Machines (SFM)
#### Moore type
The output only depends on the present state the circuit.
For example, only relying on one output - 'Q'
![[Pasted image 20240220085851.png]] 
![[Pasted image 20240220090052.png]]
**The next state can be present at the output when we have a second clock.**
![[Pasted image 20240220090249.png]]
As the state changes, if the state does not proc over another recognisable clock-state, then the flip-flop does not trigger
![[Pasted image 20240220090521.png]]
### High-triggered D-Flip-Flop
#### Representation of two different clock cycles
![[Pasted image 20240220090839.png]]
## The nature of a finite-state machine in relation to a clock
![[Pasted image 20240220091015.png]]
## Finite-State Machine, representative of running on a clock
- Note the psuedo-Karnaugh Map
- Remember that it runs on a one-tick latter delay
- All the starting points will be 0 - **State Zero**
![[Pasted image 20240220091603.png]]
Regarding the 3 outputs that are available recognise that the system is a 2-bit system:
![[Pasted image 20240220092107.png]]
## Table representation
![[Pasted image 20240220092331.png]]
### Addendum: Truth-Table Representation
![[Pasted image 20240220092644.png]]

**Duplicated; slight update**
![[Pasted image 20240220092949.png]]
#### Nicer truth-table representation
![[Pasted image 20240220093129.png]]
**We need to find the next state's logic gate**
So we have to find the Karnaugh map for the truth-table above, and for the outputs of $Y_2$, $Y_1$, & $z$.
So we would need to use a Karnaugh Map 3 times.

$Y_2$'s Karnaugh Map; most reduced circuit
![[Pasted image 20240220093617.png]]
$Y_1$'s Karnaugh Map; most reduced circuit
![[Pasted image 20240220093657.png]]
$z$'s Karnaugh Map; most reduced circuit
![[Pasted image 20240220093942.png]]
## Finding how many Flip-Flops you need
- **It depends on the number of states.**
	- The states of both present and 'next' states will always be the same. And can be represented by using flip-flops.

## Resultant Circuit
![[Pasted image 20240220094148.png]]
Re-revealing the number of inputs we have from this figure:
![[Pasted image 20240220094401.png]]
**We have 2 inputs; which is $w$**
![[Pasted image 20240220095118.png]]
![[Pasted image 20240220095345.png]]
### The output only relies on the present-states
So the resulting circuit is a Moore's (FSM) 

#### Addendum: The sample on the slides utilised 'z' output as only a 2x2 map, rather than a 4x2
![[Pasted image 20240220095827.png]]

Resulting in only 1 gate used for Z, which is only 1 true-state from y2.

# State Practise
![[Pasted image 20240220100314.png]]
**A**: 0
**B**: The state for B doesn't change, because it already has achieved the state of '1'; 1
**C**: 
**D**: 1010; the states that are similar if the 'w' is zero, the states are smiliar
	If w=1, then the state changes to State 'B'; 1011

## J-K Truth Tables
![[Pasted image 20240220101659.png]]
![[Pasted image 20240220101707.png]]
## Finite State Machine Diagram
### "State Diagram"
![[Pasted image 20240220102613.png]]
### Inputs: 9
$A, B, C, D, E, F, G, H, w$
0000 0000 1
**512 elements**
**8 Flip-Flops**: A, B, C, D, E, F, G, H.

Typical symbolism
![[Pasted image 20240220102927.png]]

# Typical FSM Basic Design Workflow
1. State Diagram
2. State Table
3. Assign Binary #
4. Find Next State Functions; Kmaps - State Functions
5. Implement the logic gates; circuits

Refer to the above.

Hypothetical
The above design is a luggage-scanner
It scans:
**A**: Checkpoint, to return to bag
**B**: Validates the bag
**C**: Checks
**D**: Absence of Make-up
**E**: Presence of Chemicals
**F**: Absence of Guns
**G**: Sensors; Detection of Radiation (looking for absence of-)
**H**: Passes all conditions; This is the validation for presence on the plane
**$N_2$**: Measures the person of an arbitrary metric of health
**$N_1$**: From **G**,
- For animals, checking

This entire process idealises the automation, without the necessity of a human - completely handsoff.
Designing is the difficult part.

### Addendum ramble
Everywhere we use finite-state machines
- Cars
	- Car lights
	- Sensors detecting an effect to procate
	- The front bumpers have sensors
		- Exposed to high-pressure, it will tell the computer that there is an accident
		- The signal is then carried over to the airbags

Remember that the 
The finite state machine is more, if the output relies only on the present state

milli finite state machine
If the output relies on the input or moore.

![[Pasted image 20240220104137.png]]

## Reasoning for being named 'next state'
Does not have the same intuitive meaning as 'Future'-tense

But instead refers to the "Next Clock-cycle" state.

![[Pasted image 20240220104401.png]]
