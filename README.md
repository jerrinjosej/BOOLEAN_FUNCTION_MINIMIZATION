# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Jerrin Jose J RegisterNumber:212225040152*/
```
module exp2(a, b, c, d, w, x, y, z, f1, f2);

input a, b, c, d, w, x, y, z;
output f1, f2;

assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));

assign f2 = ((~y & z) | (w & y) | (x & y));

endmodule
```

**Timing diagram**

<img width="1904" height="978" alt="image" src="https://github.com/user-attachments/assets/e00184bc-6d49-41a4-bbb0-5a8e8c44745f" />

**RTL**

<img width="445" height="433" alt="Screenshot 2026-05-21 131822" src="https://github.com/user-attachments/assets/50594c98-ca95-4d7f-8a2e-b317368b6282" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

