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

![image](https://github.com/user-attachments/assets/e82d0bf9-0477-4312-b745-c9a3c2dd71d4)

FULL SUBTRACTOR

![image](https://github.com/user-attachments/assets/4f97133b-ddc5-4612-8478-49d36082c86b)

**Procedure**

1 Type the programme in Quartus software.
2 Compile and run the program.
3 Generate the RTL schematic and save the logic digram.
4 Create the RTL schematic and save the logic diagram.
5 For different input combinations generate the timing diagram.
Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 

i)FULL ADDER

module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^c);
assign carry= ( (a & b)| ( cin &(a ^ b ));
endmodule

ii)FULL SUBTRACTOR

module fs(a,b,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b )));
endmodule

Developed by: SANJAY A
RegisterNumber:24010848
*/

**RTL Schematic**

FULL ADDER

![image](https://github.com/user-attachments/assets/c815a272-c971-4849-bb4e-72c3965e71d5)

FULL SUBTRACTOR

![image](https://github.com/user-attachments/assets/ad6ed2e0-0769-4cd4-837e-1e10a3fc4380)


**Output Timing Waveform**

FULL ADDER 

![image](https://github.com/user-attachments/assets/0fbfbf9c-258f-487c-a971-f5042c01b951)

FULL SUBTRACTOR

![image](https://github.com/user-attachments/assets/87a9ec52-6364-45d4-9c38-973ddc6a952f)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



