# Source Transformation
![[Pasted image 20240415153835.png]]
Essentially the analgous same in DC

## Example
*Note: Mesh Analysis cannot be done because there is no Voltage Source*
![[Pasted image 20240415154015.png]]
$X_L = jwl = j(200)(5*10^{-3})=j\ohm$
$X_C = \frac{-j}{wc}=\frac{-j}{200(1*10^{-3})}=-j5\ohm$
$I_S = 16\angle 30\degree A$

![[Pasted image 20240415154407.png]]
$V_S = I_S * R = (16\angle 30\degree A)(5\angle 0\degree \ohm)=80\angle 30\degree V$

![[Pasted image 20240415154710.png]]
$i = \frac{V_S}{Z_{EQ}=\frac{80\angle 30\degree}{(5 + 3 + j - j5)}} = 8.944 \angle 56.8\degree A$
### Nodal Analysis
![[Pasted image 20240415154852.png]]

$\Sigma I_{in} = \Sigma I_{out}$
$I_S=I_1 + I_2$
$\frac{V}{R_1} + \frac{V}{R_2+X_L+X_C}=I_S$
$(\frac{1}{R_1}+\frac{1}{R_2+X_L+X_C})*V=I_S$
$(\frac{1}{5}+\frac{1}{3-j4})V=16\angle 30\degree$
$V=\frac{16\angle 30\degree}{\frac{1}{5}+\frac{1}{3-j4}} = 44.72\angle 3.436\degree$
$i=\frac{V}{R_2+X_L+X_C}=\frac{44.72\angle 3.436\degree}{3-j4}=8.944\angle56.56 \degree A$

## Example 2
![[Pasted image 20240415155900.png]]
### Tangent: How to find Thevenin's Equivalent
![[Pasted image 20240415155942.png]]
#### Student Set 1 & 2 work @ a&b and c&d respectively
![[Pasted image 20240415160035.png]]
![[Pasted image 20240415160152.png]]
#### Student set 1 @ a&b and Student set 2 @ c&d
![[Pasted image 20240415160432.png]]
### Tangent 2
![[Pasted image 20240415160820.png]]
#### Mesh Analysis
![[Pasted image 20240415160843.png]]
#### Voltage Divider
![[Pasted image 20240415161345.png]]
#### Current Divider
![[Pasted image 20240415161544.png]]
#### Thevenin Transformation
![[Pasted image 20240415161848.png]]
*Note: Draw the final circuit or you may lose points*
#### Example Tangent Modified
![[Pasted image 20240415162212.png]]
##### Voltage Divider
![[Pasted image 20240415162236.png]]
##### Thevenin Transformation
- 1) Short-circuit
![[Pasted image 20240415162405.png]]
- 2) Combine $Z_3 || Z_4 + Z_2$
![[Pasted image 20240415162505.png]]
- 3) Find $Z_{TH} = $Z_1 || Z_6$
![[Pasted image 20240415162600.png]]
##### Reasons:
![[Pasted image 20240415162713.png]]
Sometimes a system is broken into different sub-systems, and the system needs to be broken into pieces. It may take days to troubleshoot the system, so we break them into Thevenin Equivalent chunks, realising each pevious system is reliant on on the preceeding one; we find that it's essentially $V_{TH}$ \& $Z_{TH}$.

### Back to main example:
##### Thevenin's Transformation
![[Pasted image 20240415163104.png]]
![[Pasted image 20240415163346.png]]

#### Current Divider
![[Pasted image 20240415163814.png]]
![[Pasted image 20240415163916.png]]
### Norton Equivalent
![[Pasted image 20240415165100.png]]

##### Finding $Z_{N}$
![[Pasted image 20240415165506.png]]
##### Finding $I_N$
![[Pasted image 20240415165733.png]]
*Note: We cannot do Source Transformation as a viable technique, because we have a 'Short Circuit' in the way*
Potential Techniques:
- Nodal Analysis
- ***Mesh Analysis***
- Current Divider
##### Mesh Analysis
- 1) Establish Loops
![[Pasted image 20240415165913.png]]
- 2) Establish Polarities
![[Pasted image 20240415170004.png]]
- 3) Begin Mesh-Analysing
***Identify @ Mesh 1***
$I_1 = I_S$

***KVL @ Mesh 2***
$I_2 = V_{R_1} + V_{R_2}=0$
$R_1(I_2-I_1)+R_2I_2=0$
$-R_1I_1+(R_1+R_2)I_2$
$-70I_1+100I_2=0$

***KVL @ Mesh 3***
$V_{X_L}+V_{X_C}=0$
$X_L(I_3-I_1)+X_C*I_3=0$
$-X_L*I_1+(X_L+X_C)I_3=0$
$-j80*I_1+j50*I_3=0$

***Solving for $I_2$***
*Grab values from Mesh 2 & Mesh 1*
$100I_2=60I_1$
$I_2=\frac{(60)(3\angle 60\degree)}{100}=1.8\angle60\degree$

***Solving for $I_3$***
$j50I_3=j80I_1$
$I_3=\frac{(80\angle90\degree)(3\angle60\degree)}{50\angle90\degree}=4.8\angle60\degree$

***Solving for $I_{SC}$***
$I_{SC}=I_3-I_2=(4.8\angle60\degree)-(1.8\angle60\degree)=3\angle60\degree A$

***Final Circuit Redrawn***
![[Pasted image 20240415170856.png]]
### Example 3
![[Pasted image 20240415171120.png]]
#### Voltage Node A
![[Pasted image 20240415171245.png]]
#### Mesh Analysis
![[Pasted image 20240415171358.png]]
***Auxiliary Equation***
$V_D = 10V_X$

***Finding $V_X$***
$V_X=VR_2=R_2(I_1-I_2)=60I_1-60I_2$

***Substituting back into $V_X$***
$V_D=600I_1-600I_2$

***Mesh 1***
$V_S+VR_1+VR_2=0$
$R_1I_1+R2(I_1-I_2)=V_S$
$(R_1+R_2)I_1-R_2I_2=V_S$
$72I_1-60I_2=120$

***Mesh 2***
$VR_2+VX_C+VR_3+V_D=0$
$R_2(I_2-I_1)+X_CI_2+R_3I_2+700I_1-600I_2=0$
$(600-R_2)I_1+(R_2+R_3+X_C-600)I_2=0$
$540I_1+(-420-j40)I_2=0$

***Matrix***
![[Pasted image 20240415172136.png]]
#### Finding $I_{SC}$
![[Pasted image 20240415172332.png]]
![[Pasted image 20240415172349.png]]
#### Mesh Analysis: REDO
*Note: We do not redo mesh loop 1, since the new loop doesn't involve the $I_1$*

***Mesh 2***
$V_{R_2}+V_{X_C}+V_{R_3}+V_D=0$
$R_2(I_2-I_1)+X_CI_2+R_3(I_2-I_3)+600I_1-600I_2=0$
$(600-R_2)I_1+(R_2+R_3-600+X_C)I_2-R_3I_3=0$
$540I_1+(-420-j40)I_2-120I_3=0$

***Mesh 3***
$-V_D+V_{R_3}=0$
$R_3(I_3-I_2)-(600I_1-600I_2)=0$
$-600I_1+480I_2+120I_3=0$

***Matrix***
![[Pasted image 20240415173015.png]]