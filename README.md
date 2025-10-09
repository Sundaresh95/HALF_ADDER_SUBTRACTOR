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

<img width="459" height="466" alt="image" src="https://github.com/user-attachments/assets/6b189ea5-3e37-4780-9c41-80683a8dd12e" />




Figure -01 HALF ADDER
<img width="424" height="249" alt="image" src="https://github.com/user-attachments/assets/32b412f4-2e4e-4d73-a33a-9770f3b055e5" />

**Half Subtractor**
<img width="436" height="248" alt="image" src="https://github.com/user-attachments/assets/b3af9874-7938-453b-a907-8ae51df31339" />

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

<img width="476" height="448" alt="image" src="https://github.com/user-attachments/assets/a105dbba-e7f1-4a2f-b307-7039a5a2a1b7" />



Figure -02 HALF Subtractor
<img width="424" height="249" alt="image" src="https://github.com/user-attachments/assets/07ce7038-a355-470d-b7b8-8560fbd7858f" />

**Truthtable**
<img width="436" height="248" alt="image" src="https://github.com/user-attachments/assets/2b257363-4387-4b94-92c7-594fa04bc41a" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 module FAHA1 (a,b,c,x,y,z,sum,dif,car,bor); input a,b,c,x,y,z; output sum,dif,car,bor; assign sum = a^b^c; assign car = a&b |
 a&c | b&c; assign dif = x^y^z; assign bor = ~x&z | ~x&y | y&z; endmodule

Developed by: RegisterNumber:*/
SUndaresh/25006077

**RTL Schematic**
<img width="1136" height="690" alt="image" src="https://github.com/user-attachments/assets/f577de80-0aa8-4cd3-aacd-e5d952ddcb74" />

**Output/TIMING Waveform**
<img width="1921" height="1201" alt="image" src="https://github.com/user-attachments/assets/8b25817a-5cd2-4c2e-8716-36b1095d09f4" />

**Result:**
Thus the Half Adder and Half Subtractor are studied and the truth tables are verified
