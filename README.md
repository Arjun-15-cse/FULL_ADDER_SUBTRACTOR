**EXP4:FULL ADDER AND SUBTRACTOR**

NAME: ARJUN.K

REFERENCE NO: 24900977

**AIM**
To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

FULL ADDER

![image](https://github.com/user-attachments/assets/a80a8cc5-b16d-42b5-849e-f35dda4a66e1)


FULL SUBRACTOR

![image](https://github.com/user-attachments/assets/840f4298-3f66-4d84-b5ed-9a3d20b63c77)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Program:**

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:

FULL ADDER

module fulladder(a,b,cin,sum,carry);

input a,b,cin;

output sum,carry;

assign sum=( (a ^ b)^cin);

assign carry= ( (a & b)| ( cin &(a ^ b )));

endmodule

FULL SUBRACTOR

module fullsubractor(a,b,bin,difference,borrow);

input a,b,bin;

output difference,borrow;

assign difference= ( (a ^ b)^bin);

assign borrow= ( ( a & b)| ( bin & ((a ^ b ))));

endmodule


**RTL Schematic**

FULL ADDER

![WhatsApp Image 2024-12-04 at 16 07 53_1f018637](https://github.com/user-attachments/assets/af1f75b1-ee7d-45e1-a1c4-335cfd19359c)


FULL SUBRACTOR

![WhatsApp Image 2024-12-04 at 16 09 36_59aa61e2](https://github.com/user-attachments/assets/b2c294dd-db63-43fa-b743-1a956c25988d)


**Output Timing Waveform**

FULL ADDER

![WhatsApp Image 2024-12-04 at 16 09 00_a7b123e3](https://github.com/user-attachments/assets/05953c96-5221-47f6-84f4-27f72ec6a98f)


FULL SUBRACTOR

![WhatsApp Image 2024-12-04 at 16 10 25_34ab39e7](https://github.com/user-attachments/assets/c27dc018-47a8-4720-baf7-d8df1bac98d0)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



