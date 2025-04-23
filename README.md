# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**
REGISTER NO:212224040197
NAME:MOHANAPRABHA S
DATE:23.04.2025

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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

```
module boolean(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```



**Truth Table
![Screenshot 2025-04-23 191034](https://github.com/user-attachments/assets/32af139b-acbb-43ce-9074-a7efc96f5f82)

![Screenshot 2025-04-23 191055](https://github.com/user-attachments/assets/4798de78-5fab-4277-92be-deba955a2c79)



**RTL**


![Screenshot 2025-04-23 190546](https://github.com/user-attachments/assets/1775a16c-06e9-4550-97ba-43e85f7d7eca)

**Output:**

![Screenshot 2025-04-23 190754](https://github.com/user-attachments/assets/90c69795-4dd8-4f76-aeac-265aba2026b6)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


