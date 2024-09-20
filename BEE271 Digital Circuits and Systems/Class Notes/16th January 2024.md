Quiz Correction notes:
X+0 = X

if X=0
X'=1

if X=1
X' = 0

Imagine the 'Not'-line.

### Min-Terms & Max-Terms
While using Min-terms v.s. Max-terms, realise that 
- Min-terms
	- use SOP (Sum of Products)
	- F=m_1+m_2+m_3=Summationm(1,2,3,) -> (   ) + (    ) + (    )
	- 1 at the output
- Max-terms
	- use POS (Product of Sum)
	- F = M_3.M_5.M_7=POS(3,5,7) -> ( + ).( + ).( + )
	- 0 at the output

| Bitwise | x1 | x2 | x3 | F |
| ---- | ---- | ---- | ---- | ---- |
| 0 | 0 | 0 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 2 | 0 | 1 | 0 | 1 |
| 3 | 0 | 1 | 1 | 0 |
| 4 | 1 | 0 | 0 | 1 |
| 5 | 1 | 0 | 1 | 1 |
| 6 | 1 | 1 | 0 | 1 |
| 7 | 1 | 1 | 1 | 0 |

Karnaugh Map
## Min-Terms
|  | x'1 | x1 |
| ---- | ---- | ---- |
| x'2 | m0 | m2 |
| x2 | m1 | m3 |

|  |  | 00 | 01 | 11 | 10 |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  | x'1 | x'1 | x1 | x1 |
| 0 | x'3 | m0 | m2 | m6 | m4 |
| 1 | x3 | m1 | m3 | m7 | m5 |
|  |  | x'2 | x2 | x2 | x'2 |

|  | x'1 | x'1 | x1 | x1 |  |
| ---- | ---- | ---- | ---- | ---- | ---- |
| x'3 | m0 | m4 | m12 | m8 | x'4 |
| x'3 | m1 | m5 | m13 | m9 | x4 |
| x3 | m3 | m7 | m15 | m11 | x4 |
| x3 | m2 | m6 | m14 | m10 | x'4 |
|  | x'2 | x2 | x2 | x'2 |  |
### Class Sample
|  | x'1 | x'1 | x1 | x1 |
| ---- | ---- | ---- | ---- | ---- |
| x'3 | ==1== | ==1== | ==1== | **==1==** |
| x3 | 0 | 0 | 0 | **1** |
|  | x'2 | x2 | x2 | x'2 |
F' = m_1 + m_3 + m_7
F' = X'1.X3 + X2.X3
F=F''= (X'1.X3+X2.X3)' = (X1'X3)'.(X2X3)'=(X1+X'3).(X'2+X'3)
![[Pasted image 20240116093003.png]]
(Top Circuit: Min, Bottom Circuit: MAX)

F''= (X'3+X1.X'2)''
   = ((X'3.(X'1X'2)))'
   \= (X3.(X1X1)) 

#### Order of Best Minimization
1. Karnaugh Maps
2. Logic Parse

|  | x'1 | x1 |
| ---- | ---- | ---- |
| x2 | 1 | 0 |
| x'2 | 0 | 0 |
Min: X'1.X2 (Preferable): F' = m1+m(...)
MAX: F = F''
*Case Equation:* F= m0

|  | x'1 | x1 |
| ---- | ---- | ---- |
| x2 | **1** | 0 |
| x'2 | ==**1**== | ==1== |
*Case Equation:* F = m0 + m1 + m3

|  | x'1 | x'1 | x1 | x1 |
| ---- | ---- | ---- | ---- | ---- |
| x3 | 1 | 0 | 1 | 0 |
| x'3 | 0 | 1 | 0 | 1 |
|  | x'2 | x2 | x2 | x'2 |
*Case Equation:* F = m9 + 

|  | x'1 | x'1 | x1 | x1 |
| ---- | ---- | ---- | ---- | ---- |
| x3 | 1 | 0 | 1 | 1 |
| x'3 | 0 | 1 | 0 | 1 |
|  | x'2 | x2 | x2 | x'2 |

# Karnaugh Map Laws
- Must be circled in bit-wise logic, so in 1, 2, 4, or 8s
- Must be circled adjacently; in squares
- Circling map overlap
- You are allowed to circle over the repeating boundary box
### Purpose of the Karnaugh Map
- Minimising Circuits
- Reducing code complication
- Reducing gate size
### Karnaugh Map Footnotes
- The number of gates include the
	- Circled gates; which are as many as circled
	- And the last gate that encompasses the entire circuit logic
	- Summation of Nth+1

##### The Karnaugh Table results as 1, which is connected directly to the source
|  | x'1 | x'1 | x1 | x1 |
| ---- | ---- | ---- | ---- | ---- |
| x2 | 1 | 1 | 1 | 1 |
| x'2 | 1 | 1 | 1 | 1 |
|  | x'3 | x3 | x3 | x'3 |
![[Pasted image 20240116094723.png]]

##### The Karnaugh Table results as 0, which is connected directly to ground
|  | x'1 | x'1 | x1 | x1 |
| ---- | ---- | ---- | ---- | ---- |
| x2 | 0 | 0 | 0 | 0 |
| x'2 | 0 | 0 | 0 | 0 |
|  | x'3 | x3 | x3 | x'3 |
![[Pasted image 20240116094823.png]]
### Finding Karnaugh Map MAX-TERMS

1. FIND
2. CIRCLE
3. COMPLIMENT
4. POS
# "Suppose you don't have a Karnaugh Map"
### AND TO QUOTE THE GREAT BASERE, "USE KARNAUGH MAPS"
##### "NO ONE CAN FORCE YOU TO USE *THAT* TECHNIQUE"
# Textbook Recc by Basere
#### Digital Systems, by Minmorss