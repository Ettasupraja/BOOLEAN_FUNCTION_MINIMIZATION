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

Developed by: RegisterNumber:*/212223220022
module BooleanMinimization(A,B,C,D,F1); 
input A,B,C,D; 
output F1; 
wire x1,x2,x3,x4,x5; 
assign x1=(~A)&(~B)&(~C)&(~D); 
assign x2=(A)&(~C)&(~D); 
assign x3=(~B)&(C)&(~D); 
assign x4=(~A)&(B)&(C)&(D); 
assign x5=(B)&(~C)&(D); 
assign F1=x1|x2|x3|x4|x5; 
endmodule
![WhatsApp Image 2024-04-01 at 09 28 11_36592374](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/550838f8-8dbc-48ae-b57e-fcb457f0a062)


**RTL realization**
![WhatsApp Image 2024-04-01 at 09 28 23_30d1249d](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/4a06fe61-8e3c-4f94-baed-6b901e106994)


**Output:**

![WhatsApp Image 2024-04-01 at 09 28 35_053f766c](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/045f0ecc-0558-4171-b230-d00fea380b42)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

