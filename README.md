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


Half Adder

![half-adder-truth-table](https://github.com/user-attachments/assets/a302fecb-2489-4e23-8be2-18a3bd1bb390)

Half Subtractor

![half-subtractor2](https://github.com/user-attachments/assets/169b3e9a-cdc1-485a-8778-5e51329d8570)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:S ABINAV AADITYA
RegisterNumber:24002354
***
program of half adder:

module haaaa(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= ( a ^ b);

assign carry =(a & b);

endmodule
***


***
program of half subtractor:

module hasub(a,b,diff,borr);

input a,b;

output diff,borr;

assign diff= (a^b);

assign borr= (~a&b);

endmodule
***
**RTL Schematic**


Half Adder

![ha add](https://github.com/user-attachments/assets/c148f88d-02f4-4159-90ba-973600943f19)

Half Subtractor

![ha sub](https://github.com/user-attachments/assets/fe2ba5ce-adf0-4402-9d60-fa80a8aef95b)

**Output/TIMING Waveform**



Half Adder


![ha add (2)](https://github.com/user-attachments/assets/fb76aefd-d66f-4086-9e6c-55c0fe50357f)

Half Subtractor

![ha sub (2)](https://github.com/user-attachments/assets/6daeb80b-bd51-4f5a-a9c2-777e4bc43826)


**Result:**
Thus designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.
