

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
module logic_function(
    input a, b, c, d,
    input w, x, y, z,
    output f1, f2
);

assign f1 = (~b & ~d) | (a & b & ~c) | (~a & b & d);
assign f2 = (~y & z) | (x & y) | (w & y);

endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**

**Output:**
<img width="870" height="986" alt="523905850-c15b4d5f-81c3-495f-ab2d-37d6dd282f01" src="https://github.com/user-attachments/assets/e71697c9-1a59-4d14-b617-b05cb465c0d6" />

**RTL**

**Timing Diagram**
<img width="1917" height="595" alt="523905890-10e5fd21-a8b6-41b0-aca6-c24b04ded38b" src="https://github.com/user-attachments/assets/6d34cc1e-4fdf-4fd6-a2d7-b421ddc8cc23" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

