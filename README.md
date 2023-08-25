# Experiment-02 Implementation of combinational logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
#### OR Gate:
The OR gate is a fundamental digital logic gate that operates on two binary inputs, producing an output of 1 if at least one input is 1. It symbolizes logical disjunction and is essential in building logical circuits and decision-making processes in computers and electronics.
#### AND Gate:
The AND gate is a fundamental digital logic gate with two inputs and one output. It produces a high output (1) only when both input signals are high (1). If any input is low (0), the output remains low. It's a building block for more complex logic circuits and is integral in digital computations.
#### NOT Gate:
The NOT gate is a fundamental digital logic gate. It has a single input and a single output. The output is the inverse of the input: if the input is high (1), the output is low (0), and vice versa. It's a basic building block in digital circuits, used for logic inversion.

## Procedure:
1.Create a project with required entities.
2.Create a module along with respective file name.
3.Run the respective programs for the given boolean equations.
4.Run the module and get the respective RTL outputs.
5.Create university program(VWF) for getting timing diagram. 
6.Give the respective inputs for timing diagram and obtain the results.
## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Sabari Akash A 
RegisterNumber: 212222230124 
```
module expression(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL Daigram:
![WhatsApp Image 2023-08-25 at 09 45 04](https://github.com/Sabariakash22009103/Experiment--02-Implementation-of-combinational-logic-/assets/119390227/3ba70300-859a-4bf0-83ba-641ac9059688)

## Truth Table:
![image](https://github.com/Sabariakash22009103/Experiment--02-Implementation-of-combinational-logic-/assets/119390227/16b15809-65a8-472b-af24-a74c67f8c0c2)

## Output Waveform:
![WhatsApp Image 2023-08-25 at 09 45 37](https://github.com/Sabariakash22009103/Experiment--02-Implementation-of-combinational-logic-/assets/119390227/099aa536-e439-4510-aa30-605d78d7105d)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
