# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module logic_function (a, b, c, d, w, x, y, z, f1, f2);

input a, b, c, d;
input w, x, y, z;
output f1, f2;

assign f1 = (~b & ~d) | (a & b & ~c) | (a & b & d);
assign f2 = (~y & z) | (x & y) | (w & z);

endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:25017232


**RTL realization**

**Output:**
<img width="1919" height="1079" alt="Screenshot 2025-11-19 165001" src="https://github.com/user-attachments/assets/0d0b129e-b243-44c0-bf38-cb5386a853b1" />

**RTL**
<img width="1920" height="1080" alt="Screenshot (85)" src="https://github.com/user-attachments/assets/c13ea4ea-4081-4142-8e00-592179ad7f2d" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

