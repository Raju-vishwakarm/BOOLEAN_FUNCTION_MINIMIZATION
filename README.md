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
i)module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii) module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:D.Raju RegisterNumber:24003778


**RTL realization**
![Screenshot 2024-12-29 154455](https://github.com/user-attachments/assets/3f621ae6-d6b4-4e84-bea5-2483096d2f66)
![Screenshot 2024-12-29 154523](https://github.com/user-attachments/assets/bc04c92d-918c-4d02-aff4-17843c36b827)

**Output:**

**RTL**

**Timing Diagram**
![Screenshot 2024-12-29 154537](https://github.com/user-attachments/assets/8de79692-ece9-4a9a-a82b-677a0e14ffa9)
![Screenshot 2024-12-29 154555](https://github.com/user-attachments/assets/d04af8a7-dc85-44c9-9c74-60c30c2bb059)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
