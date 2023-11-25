# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: LATHIKA L.J
RegisterNumber: 23012411 
*/

##OUTPUT:

## Code:

/*
Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
Developed by: SANJAY S
RegisterNumber: 212222230132 
module verilog1(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire  A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1= (~a&(~b)&(~c)&(~d));
assign A2= (a&c&(~d));
assign A3= ((~b)&c&(~d));
assign A4= (~a&b&c&d);
assign A5= (b&(~c)&d);
assign F1= A1|A2|A3|A4|A5;
assign B1= (x&(~y)&z);
assign B2= (~x&(~y)&z);
assign B3= (~w&x&y);
assign B4= (w&(~x)&y);
assign B5= (w&y&z);
assign F2= B1|B2|B3|B4|B5;
endmodule

## Truth table:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/d3c49bd1-68e5-464b-b0f0-4c3d1fcf3d79)

## RTL Diagram:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/13a304d7-7036-4067-a3ad-05a98c4c8e3e)

## Timing Diagram:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/08c3edfd-0245-4d9f-a5e6-88c32b89f029)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
