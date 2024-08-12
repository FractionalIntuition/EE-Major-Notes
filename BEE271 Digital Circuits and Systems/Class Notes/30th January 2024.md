# 5-bit Karnaugh Map
![[January 30 2024.jpg]]
## For an AND gate
There are no different types - we only have one generic type. Inside the circuit, or outside the gate, same thing with an OR, XAND, and NOR gate. The components do not change.

## Multi-bit Addition/Subtraction explanation
$(1010)_2 = (10)_{10}$
$-(0110)_2=-(6)_{10}$
-----------------
$1001\space\space\space\space\space(4)_{10}$
### Combination Circuit
Depends on value of output and is time-independent logic (independent of the input)
### Sequential Circuit
Only present values of the inputs but also on the past behaviour of the circuit (dependent of the inputs)

### Multiplexers
We have multiple inputs, and the output must be 1 at a time. **Only 1**
- This is done through selectors
Assumption:
Presume we have an internal switch that can configure an input/output
It chooses the sequence for 
- 1st A; 0000
- 2nd C; 0001
- 3rd B; 0010
Only one output can occur at a time; the combinations mirror the truth-table presented to us
![[Untitled 6.jpg]]

A real world example of a Multiplexer
During a landline, we do not have any delay or interference because we have multiple lines giving and receiving a single connection (output)

$F=m_2+m_3+m_5+m_7$
$F = \bar{s}x_1\bar{x_2}+\bar{s}x_1x_2+s\bar{x_1}x_2+sx_1x_2$
![[Untitled 7 1.jpg]]

# Sample
![[Untitled 8 1.jpg]]

# Mid-term Info
### Next Week
Coverage:
Sequential Circuits, but won't be on Exam

Tuesday:
Problem-sets work-together
Midterm Review

Thursday:
Midterm