# HALF_ADDER_SUBTRACTOR
Implementation-of-Half-Adder-and-Half Subtractor-circuit

AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

<img width="459" height="466" alt="image" src="https://github.com/user-attachments/assets/f8203e1e-b984-4927-bc41-8a984a9cfcb5" />


Figure -01 HALF ADDER

Half Subtractor

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B

<img width="476" height="448" alt="image" src="https://github.com/user-attachments/assets/bba524a6-3a61-48c1-8619-e4a78d08a961" />


Figure -02 HALF Subtractor

Truthtable HALF ADDER

<img width="424" height="249" alt="image" src="https://github.com/user-attachments/assets/9cbde552-3225-42c3-817f-31adb8cb6d00" />


HALF SUBTRACTOR

<img width="436" height="248" alt="image" src="https://github.com/user-attachments/assets/ac921867-c232-4c76-985d-e4122889c1e1" />


Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:

Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by:KABELAN G K 
RegisterNumber:24900985

Half Adder

module half_adder(sum, carry, a, b);
  output sum;
  output carry;
  input a;
  input b;
  assign sum = a ^ b;
  assign carry = a & b;
endmodule

Half Subtractor

module half_subtractor(diff, borrow, a, b);
  output diff;
  output borrow;
  input a;
  input b;
  assign diff = a ^ b;
  assign borrow = ~a & b;
endmodule

RTL Schematic 
<img width="1136" height="690" alt="image" src="https://github.com/user-attachments/assets/b83b5558-31ac-40fd-9091-de34ca096ee8" />


Half Subtractor 
<img width="1206" height="671" alt="image" src="https://github.com/user-attachments/assets/93212c7a-45b1-4fa3-b4ed-f3ce9c8389ca" />


Output/TIMING Waveform Half Adder 
<img width="1921" height="1201" alt="image" src="https://github.com/user-attachments/assets/111bd365-a56e-461d-bf2e-31b745bba020" />


Half Subtractor 
<img width="1921" height="1199" alt="image" src="https://github.com/user-attachments/assets/82ed4481-f1eb-41e0-ab4b-6fde19daeff0" />


Result:

Thus the Half Adder and Half Subtractor are studied and the truth tables are verified
