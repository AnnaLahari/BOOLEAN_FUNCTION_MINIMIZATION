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

Developed by:A.Lahari
RegisterNumber:212223230111 */
```
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
```
![Screenshot 2024-03-25 092512](https://github.com/AnnaLahari/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365425/617a27af-0260-406a-a4d6-65588414c509)


**RTL realization**:

![Screenshot 2024-03-25 092540](https://github.com/AnnaLahari/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365425/e6652b0a-c99f-4965-b685-6e8e0fb27ee4)

**Output:**

![Screenshot 2024-03-25 092757](https://github.com/AnnaLahari/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365425/3c6953c6-d376-410a-90e5-6433ae75fa51)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

