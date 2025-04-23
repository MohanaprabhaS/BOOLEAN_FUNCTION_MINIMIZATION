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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Mohanaprabha.S

RegisterNumber: 212224040197
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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


**Truth Table**

![Screenshot 2025-04-23 141926](https://github.com/user-attachments/assets/8c8faea7-95ca-4a33-a0df-93fb52856858)
![Screenshot 2025-04-23 141932](https://github.com/user-attachments/assets/ca96e5e7-93b8-4582-b4c9-86cfe209cf03)

**RTL**

![Screenshot 2025-04-23 141950](https://github.com/user-attachments/assets/41908d15-5161-4fcb-b053-130fa798c9c4)

**Output:**

![Screenshot 2025-04-23 142000](https://github.com/user-attachments/assets/a1d67178-ebb3-4cb3-9e77-cadd50e2c2b0)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


