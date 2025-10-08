# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

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
![498356879-8e413a7b-cc32-4b8b-9fc2-4dadfb58f17e](https://github.com/user-attachments/assets/62589cbf-ec71-4369-9f64-a2072f893b9f)

FULL SUBTRACTOR
<img width="340" height="148" alt="image" src="https://github.com/user-attachments/assets/cc9a6c82-67c1-47e1-8e9a-a20802ecc50e" />

**Procedure**

Write the detailed procedure here

**Program:**
FULL ADDER:

module exp4(a,b,cin,sum,carry); input a,b,cin; output sum,carry; assign sum=( (a ^ b)^cin); assign carry= ( (a & b)| ( cin &(a ^ b ))); endmodule

FULL SUBTRACTOR:

module fs(a,b,bin,difference,borrow); input a,b,bin; output difference,borrow; assign difference= ( (a ^ b)^bin); assign borrow= ( ( a & b)| ( bin & ((a ^ b )))); endmodule /* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

DEVELOPED BY: ANURANJAN.B

REGISTER NUMBER:25003110

**RTL Schematic**

FULL ADDER:

<img width="1919" height="1079" alt="498311531-3625b807-ce23-416d-bb79-d1a5b147553d" src="https://github.com/user-attachments/assets/cbf5e34d-d1c9-462b-a067-cab213073583" />

FULL SUBTRACTOR:

<img width="1919" height="1079" alt="498318096-9e250c73-87ad-4421-9bf4-8910e0fd5315" src="https://github.com/user-attachments/assets/03fe0d85-cf6d-4731-9634-56300927fa69" />

**Output Timing Waveform**

FULL ADDER:

<img width="1919" height="1079" alt="498311562-421227e6-fdaa-4084-91af-ce70fbecd254" src="https://github.com/user-attachments/assets/eeeddb23-7a50-4d0d-8276-e49db816a613" />

FULL SUBTRACTOR:

<img width="1919" height="1079" alt="498318097-823937a7-e054-46a1-b464-30f2a83dfe6c" src="https://github.com/user-attachments/assets/b8c5a282-8cee-4d48-84e2-bd25f6578501" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



