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
```
Developed by:AHAMED JASEER SHA .E RegisterNumber:212224040015
```
```
module
sample2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&
(~c)&(~d))|(~b)&c&(~d)|((~a)&b&c&d)|
(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|
((~w)&x&y)|(w&x&(~y))|(w&x&y);
endmodule
```


**RTL realization**

![image](https://github.com/user-attachments/assets/74cb0570-8b78-4e10-8705-c8d1440a81e5)

**Output:**

![image](https://github.com/user-attachments/assets/7cd43651-a601-414e-9453-1b7818b83704)


**Timing Diagram**

 
 ![image](https://github.com/user-attachments/assets/1004d351-7b9c-47ec-993a-c6e161a8dac5)

![image](https://github.com/user-attachments/assets/cc43ea5c-3fd9-4029-a466-745d9ca1b1d7)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

