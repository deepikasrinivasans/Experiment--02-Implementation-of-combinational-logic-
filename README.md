## NAME: DEEPIKA S
## REGISTER NUMBER: 212222230028
# Experiment 02 Implementation of combinational logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
## EQUIPMENTS REQUIRED:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
#### OR Gate:
The OR gate is a fundamental digital logic gate that operates on two binary inputs, producing an output of 1 if at least one input is 1. It symbolizes logical disjunction and is essential in building logical circuits and decision-making processes in computers and electronics.
#### AND Gate:
The AND gate is a fundamental digital logic gate with two inputs and one output. It produces a high output (1) only when both input signals are high (1). If any input is low (0), the output remains low. It's a building block for more complex logic circuits and is integral in digital computations.
#### NOT Gate:
The NOT gate is a fundamental digital logic gate. It has a single input and a single output. The output is the inverse of the input: if the input is high (1), the output is low (0), and vice versa. It's a basic building block in digital circuits, used for logic inversion.
## PROCEDURE:
 


## PROGRAM:
```
Developed by: Deepika.S
RegisterNumber:  212222230028
```
```
module EX02(A,B,C,D,F1);
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
## RTL DIAGRAM:
![rtl viewer](https://github.com/deepikasrinivasans/Experiment--02-Implementation-of-combinational-logic-/assets/119393935/086d3cf1-23a1-4853-b9c7-116ed8c5583e)
## TRUTH TABLE:
![WhatsApp Image 2023-08-25 at 9 22 38 AM](https://github.com/deepikasrinivasans/Experiment--02-Implementation-of-combinational-logic-/assets/119393935/6bef0fc3-1701-4d10-bc25-16341339eacb)
## OUTPUT WAVEFORM VERIFIED:
![WhatsApp Image 2023-08-25 at 9 22 37 AM](https://github.com/deepikasrinivasans/Experiment--02-Implementation-of-combinational-logic-/assets/119393935/209ba492-6b93-4c81-9aea-3ab948a6bb92)
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
