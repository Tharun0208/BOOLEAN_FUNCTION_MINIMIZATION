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

    1)
    module logic_function(a,b,c,d,f1);
    input a,b,c,d;
    output f1;
    assign f1=((~b & ~d)|(~a&b&d)|(a&b&~c));
    endmodule
    2)
    module EXP2(w,x,y,z,f2);
    input w,x,y,z;
    output f2;
    assign f2=((~y & z)|( w & y )|(x & y));
    endmodule
 
Developed by:Tharun.R RegisterNumber:212224240172

**Truthtable**

![image](https://github.com/user-attachments/assets/b907b2d2-608d-4cee-bd55-b72f249c37ea)
![image](https://github.com/user-attachments/assets/b49b52b3-d952-499a-916a-d3d3a15a5330)


**RTL realization**

![image](https://github.com/user-attachments/assets/f2ff029c-8eb9-4d41-94d8-af1ab9ac65f6)
![image](https://github.com/user-attachments/assets/c4ff03e3-2853-4f07-a219-ae5d4f5ac5c3)

**RTL**

![image](https://github.com/user-attachments/assets/8ec6f891-6670-4150-8e0c-ed8d49215789)
![image](https://github.com/user-attachments/assets/8afd63dc-44a5-490a-91bc-b57f1f369fb1)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

