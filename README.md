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

Developed by: S.Pavithra 
RegisterNumber:212223220073

```
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
```
**Truthtable**
![image](https://github.com/Pavithrasaravanakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/150664013/971719e6-3d36-48eb-9b28-7a6377c28ebd)



**Output:**
![image](https://github.com/Pavithrasaravanakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/150664013/99e7280b-ba5b-4ca7-9171-8dca3d7fedf8)

**RTL**

**Timing Diagram**
![image](https://github.com/Pavithrasaravanakumar/BOOLEAN_FUNCTION_MINIMIZATION/assets/150664013/67ba0f07-a436-4fa8-a242-d2403bd55c10)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

