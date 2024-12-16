# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![ex3 (2)(4) jpg](https://github.com/user-attachments/assets/4b51db52-6f4b-408f-b692-3def24e08a00)

![ex3 (2)(5) jpg](https://github.com/user-attachments/assets/c71738b9-5fd9-4628-a8d8-3eac9e80c923)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
HALF ADDER
![ex3 (3)](https://github.com/user-attachments/assets/4f9200fd-a2b5-4a0f-9dd5-3877152bf786)

HALF SUBTRACTOR
![HALF SUB EX 3](https://github.com/user-attachments/assets/9c5c10b5-9426-41e2-aac3-6f979e21904d)

Developed by: SAHITH M
RegisterNumber: 24000251

**RTL Schematic**

**HALF ADDER**
```
module halfadder (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= (a & b);
endmodule
```
***HALF SUBTRACTOR***
```
module (ha a,b,diff,borr;
input a,b;
output diff,borr;
assign diff=(a^b);
assign borr=(`a&b);
endmodule
```
HALF SUBTRACTOR
![ex3 (2)(2) jpg](https://github.com/user-attachments/assets/fed71a2a-3845-4297-b718-da2729e364c0)

**Output/TIMING Waveform**
![ex3 (2)(3) jpg](https://github.com/user-attachments/assets/c2fa17ca-3ef0-42f0-89bf-53075b9a513d)

![ex3](https://github.com/user-attachments/assets/c6a3f406-6471-4ce4-9398-72aa6b82940d)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using
Verilog programming.
