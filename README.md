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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: V.Anisha
RegisterNumber:212224040023  */
f1
```
module BFM(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

```
f2
```
module BFM1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|(w & y)|(x & y));
endmodule

```

**RTL realization**
f1
![image](https://github.com/user-attachments/assets/6185465b-5a56-4afa-8e65-9673b7a900d8)

f2
![image](https://github.com/user-attachments/assets/a5d5cc53-9717-431c-a485-835f5c8d8676)


**Timing Diagram**
f1
![image](https://github.com/user-attachments/assets/28d6ceec-f7c4-4673-88f8-204bc6642370)

f2
![image](https://github.com/user-attachments/assets/e1c82c7a-5732-4ce0-a473-3c5e71b0847d)

**Truth Table**
f1
![WhatsApp Image 2025-04-23 at 14 53 04_c5cfe925](https://github.com/user-attachments/assets/4a707cc2-5202-4fa9-8db0-f567cdf2118d)

f2
![image](https://github.com/user-attachments/assets/6e9f86d6-7ec9-4f4f-85ad-3b9c6e46f130)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

