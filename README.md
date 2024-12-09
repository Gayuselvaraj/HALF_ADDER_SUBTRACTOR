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
![WhatsApp Image 2024-12-09 at 06 41 57_553ba6b6](https://github.com/user-attachments/assets/a43823ea-65ea-4241-a673-c0373c7355c3)
Half subractor:
![WhatsApp Image 2024-12-09 at 06 42 25_3bca816c](https://github.com/user-attachments/assets/ab32134a-53c6-4a77-b9e2-85fa197ead3b)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:*/

**RTL Schematic**
Half adder:![Screenshot_2024-11-11_232329 1](https://github.com/user-attachments/assets/3aa9575c-e42c-4aff-8618-5b06bfeebb4f)

Half subractor:![Screenshot_2024-11-11_232840 1](https://github.com/user-attachments/assets/fca30790-1ed5-4d26-956a-b7b752dea4d1)


**Output/TIMING Waveform**
Half adder:![WhatsApp Image 2024-12-09 at 06 40 36_a4089b50](https://github.com/user-attachments/assets/c4f13e9d-24b2-47fa-be46-bf3da4dffeab)


Half subractor:![WhatsApp Image 2024-12-09 at 06 40 57_0ad9b1a5](https://github.com/user-attachments/assets/751924bd-2861-4cd3-b8a2-9932c2f8e766)


**Result:** : Thus the truth table of half adder and half subtractor in QuartusII using Verilog
programming is verified.
