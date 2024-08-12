Presuming under this verilog operator example
a = 4'b0101 = 5, b=3'b011 - 3

$a==b = 0$
$a!=b = 1$
$-a = -5$; Arithmetic complement
$+a = 5$; Unary plus
$a*b = 15$; Multiplication 
$a/b = 1$; Integer division
$a\%b=2$; Modulo (Remainder) Division

Shifting
$a>>b=0000$; Shifting a right b bits
$a<<b=1000$; Shifting a left b bits

Assuming
a = 3'b010
b = 3'b011
c = 3'b101

Concatenation and Replication
{a,b} Concatenate a and b    010011
{b{a}} Replicate and concatenate b (3) copies of a. b must be a constant. 010010010; 3 copies of "a"

Conditional (Trinary)
a?b:c 

*reg* keyword is a verilog output that is stored in a register (memory cell).

```verilog
module Mux2To1(s,a,b,f)
	input logic s,a,b;
	output logic f;
```
```verilog
//behavioural specifications
module example5(x1,x2,s,f)
	input x1,x2,s;
	output f;
	reg f;

always @ (x1,x2,s)
	if (s==0)
		f=x1;
	else
		f=x2;
endmodule

\\behavioural specifications II
module example5(input x1, x2, s, output reg f)
	always @(x1,x2,s)
		if(s==0)
			f=x1;
		else
			f=x2;
endmodule
```
```verilog
module Mux2To1(s,a,b,f);
	input s,a,b;
	output reg f;
always @(*)
	if(s)
		f=b;
	else
		f=a;
endmodule
```