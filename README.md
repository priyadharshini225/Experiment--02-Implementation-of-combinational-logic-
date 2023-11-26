# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
 

## Logic Diagram (using nand gate) and (using nor gate):
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/71126584-7d7f-4231-b4bb-b38495e0c1db)
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/1a4f2e2f-36d3-49a5-b98b-166451e349f2)

## Procedure:
*Create a project with required entities.
*Create a module along with respective file name. 
*Run the respective programs for the given boolean equations.
*Run the module and get the respective RTL outputs.
*Create university program(VWF) for getting timing diagram.
*Give the respective inputs for timing diagram and obtain the results.
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: PRIYADHARSHINI S
RegisterNumber: 23003522
module combinational(a,b,c,d,w,x,y,z,fl,f2);
input a,b,c,d,w,x,y,z;
output fl,f2;
wire g1=((~a)&(~b)&(~c)&(~d)); 
wire g2=((a)&(~c)&(~d));
wire g3=((~b)&(c)&(~d));
wire g4=((~a)&(b)&(c)&(d)); 
wire g5=((b)&(~c)&(d));
assign fl=g1|g2|g3|g4|g5; 
wire g6=((x)&(~y)&(z));
wire g7=((~x)&(~y)&(z));
wire g8=((~w)&(x)&(y)); 
wire g9=((w)&(~x)&(y));
wire g10=((w)&(x)&(y)); 
assign f2=g6|g7|g8|g9|g10;
endmodule
*/

## Output:
## RTL realization of NAND AND NOR gates:
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/4f83aa40-3884-45c0-b9c7-2d8abca495aa)
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/7ebd6c85-2385-4ef6-8c7f-c127f2ebb1d0)

## Truthtable of NAND gate:
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/24364ce7-4c4e-4482-951d-394a31e2cbf0)
## Truthtable of NOR gate:
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/bfd0a856-c799-472e-a543-a7987bbc5304)

## Timing Diagram:
![image](https://github.com/priyadharshini225/Experiment--02-Implementation-of-combinational-logic-/assets/138849213/b12d744e-2043-42ad-adc7-96d70c2a7c71)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
