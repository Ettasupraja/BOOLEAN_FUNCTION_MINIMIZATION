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

Developed by:ETTA SUPRAJA
RegisterNumber: 212223220022*/ 
module combinationalcircuit(A,B,C,D,F1);
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
![Screenshot 2024-04-04 164024](https://github.com/Ettasupraja/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/a2c0e4d4-84d7-4cd7-ad13-52a02958f2a4)


**RTL realization**
![Screenshot 2024-04-04 164048](https://github.com/Ettasupraja/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/f303b6fc-1bab-442c-ae2a-ff0d9a289890)


**Output:**
![Screenshot 2024-04-04 164059](https://github.com/Ettasupraja/BOOLEAN_FUNCTION_MINIMIZATION/assets/151641352/3015c3f4-3a93-44df-8a76-4dab4e5ba9c9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

