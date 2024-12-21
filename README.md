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

**Truthtable**:
Half adder:



![397930368-6917253e-4b99-4d73-99d4-ca83a8835326](https://github.com/user-attachments/assets/50609517-6f50-4014-ad8a-e278a900ae2d)


Half subractor:

![397930376-db04186a-6e78-4da3-bbf2-98ef7c5896e6](https://github.com/user-attachments/assets/14858163-01fc-4c2c-bca0-7c876ae58805)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Gayathri S 

RegisterNumber:24900444

```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```


**RTL Schematic**

Half adder:


![Screenshot_2024-11-11_232329 1](https://github.com/user-attachments/assets/3aa9575c-e42c-4aff-8618-5b06bfeebb4f)

Half subractor:

![Screenshot_2024-11-11_232840 1](https://github.com/user-attachments/assets/fca30790-1ed5-4d26-956a-b7b752dea4d1)


**Output/TIMING Waveform**

Half adder:


![392862681-4f0a4ecc-62d8-4c2b-8e90-b291698d5940](https://github.com/user-attachments/assets/2aa04412-bd7c-4a1f-8ad7-a7c4fb4f1471)




Half subractor:


![392862720-76da6dd6-e373-4956-b355-0659a42b3597](https://github.com/user-attachments/assets/1220038c-c1f2-4d2e-b7df-ab4d5ad8ac17)




**Result:** : Thus the truth table of half adder and half subtractor in QuartusII using Verilog
programming is verified.
