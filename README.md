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
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Using NAND gates
NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Using NOR GATES
NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Logic Diagram
![image](https://github.com/JoyceBeulah/Experiment--02-Implementation-of-combinational-logic-/assets/118343698/0b49e589-62a9-4f98-898e-9bb525265e89)

## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: R.Joyce Beulah
RegisterNumber:  212222230058
*/
## RTL 
NAND combination :

![image](https://github.com/JoyceBeulah/Experiment--02-Implementation-of-combinational-logic-/assets/118343698/17d3a272-62ac-4dd7-beeb-da6522cad07e)

NOR combination :

![image](https://github.com/JoyceBeulah/Experiment--02-Implementation-of-combinational-logic-/assets/118343698/211c6291-ee50-471c-a35b-63f3018f407a)

## Timing Diagram
NAND combination :

![image](https://github.com/JoyceBeulah/Experiment--02-Implementation-of-combinational-logic-/assets/118343698/45deb2ca-5915-4011-befd-1b357af6b267)


NOR combination :

![image](https://github.com/JoyceBeulah/Experiment--02-Implementation-of-combinational-logic-/assets/118343698/b5924734-36b6-482c-95f1-a16f5411b0bf)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
