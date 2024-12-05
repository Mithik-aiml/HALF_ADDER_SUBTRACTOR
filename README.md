# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

NAME:G.MIHIK JAIN

REF NO:24001881

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
HALF ADDER:
![half-adder truth table](https://github.com/user-attachments/assets/8a81f762-0f2d-4fc9-a309-e8b1fa1c4928)

HALF SUBRACTOR:
![image](https://github.com/user-attachments/assets/b18963e2-91ab-42a7-bce3-f5b93afca5ed)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER:
module half_adder_structural(
input a,//Input'a'
input b,//Input'b'
output s,//Output's'(Sum)
output c//Output'c'(Carry)
);
xor gate_xor(s,a,b);//XOR gate for sum
and gate_xor(c,a,b);//AND gate for carry
endmodule

HALF SUBRACTOR:
module halfsub(diff,borr,a,b);
input a,b;
output diff,borr;
wire w1;
xor g1(diff,a,b);
not g2(w1,a);
and g3(borr,w1,b);
endmodule

**RTL Schematic**

HALF ADDER:
![image](https://github.com/user-attachments/assets/49644bd5-7de4-422f-9e66-ea4ffd7aeef3)

HALF SUBRACTOR:
![half sub rtl](https://github.com/user-attachments/assets/a5656e87-f51d-4bf4-8fdb-9afca076368e)

**Output/TIMING Waveform**
HALF ADDER:
![Screenshot 2024-12-05 115502](https://github.com/user-attachments/assets/3b69777a-414f-4f0e-9764-6a2be136f23f)

HALF SUBRACTOR:
![half sub output](https://github.com/user-attachments/assets/c3f4b554-eff2-4274-af71-ff6489cc9e2d)

**Result:**

Thus we design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.
