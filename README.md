# HALF_ADDER_SUBTRACTOR
##DATE : 8/10/2024
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

**TRUTH TABLE**
![WhatsApp Image 2024-12-21 at 09 38 24_2d3875d2](https://github.com/user-attachments/assets/e71ab7e5-537f-4cd8-a381-6f4ed9bca9b0)

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![WhatsApp Image 2024-12-21 at 09 37 29_1f04456b](https://github.com/user-attachments/assets/f8bc31c2-297c-4600-83e3-5b2c9a18ada0)

**Procedure**

1.	Type the program in Quartus software.
2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
i)HALF ADDER

module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

```

Developed by: S HEMANTH KUMAR RegisterNumber:*/24011247

**RTL Schematic**
![Screenshot (19)](https://github.com/user-attachments/assets/1258c267-84e7-40e7-889a-105e945f96a8)
![Screenshot (22)](https://github.com/user-attachments/assets/026ffe32-d1cf-4b75-8452-1dc3661d5a14)


**Output/TIMING Waveform**
![Screenshot (20)](https://github.com/user-attachments/assets/f8355a1e-3a19-4770-b5f5-d83e3dee21cf)
![Screenshot (23)](https://github.com/user-attachments/assets/ca68e661-f7c1-4e5e-aebf-eadba860d4a7)


**Result:**
To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming is verified.
