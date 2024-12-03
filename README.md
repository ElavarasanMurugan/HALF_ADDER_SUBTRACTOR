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
1. HALF ADDER
 ![Half adder truth table](https://github.com/user-attachments/assets/9b3aed28-54a0-4a86-9007-d9d2414d8a1b)

2.HALF SUBRACTER
![half subracter truth table](https://github.com/user-attachments/assets/8eafd4c4-8d73-428d-9750-e565429e9331)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.


1.HALF ADDER

module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

2.HALF SUBRACTER

module halfsubracter(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule



Developed by: Elavarasan M RegisterNumber: 24900162*/

**RTL Schematic**
1. HALF ADDER
  ![half adder logic diagram](https://github.com/user-attachments/assets/a946b4ae-1c88-4718-828a-2d1ff39adf7c)

2. HALF SUBRACTER
 ![Halfsubracter logic diaram ](https://github.com/user-attachments/assets/bbc3df2b-bb5e-4f0a-8dcf-d571ac71a9aa)

**Output/TIMING Waveform**

1. HALF ADDER
 ![Half adder waveform](https://github.com/user-attachments/assets/5893c17d-da86-4c59-9960-bf9c72f86fa0)

2. HALF SUBRACTER

![half subracter waveform](https://github.com/user-attachments/assets/5c3a445e-1c99-49b8-8f91-bde7a2e9c4ab)

**Result:**

Thus the half adder and half subtractor circuits were successfully designed, and their truth tables were verified in Quartus using Verilog programming.
