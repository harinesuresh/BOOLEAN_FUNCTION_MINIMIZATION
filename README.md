# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

![Screenshot 2025-04-07 130650](https://github.com/user-attachments/assets/c8eed710-67b1-4ae0-a222-70604108dd9f)


**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:HARINE S
RegisterNumber: 212224230081 */

```
module exp2a(a,b,c,d,F1);
intput a,b,c,d;
output F1;
assign F1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

module exp2b(w,x,y,z,F2);
input w,x,y,z;
output F2;
assign F2=((~y&z)|(x&y)|(w&y));
endmodule
```


**RTL realization**

**Output:**

**RTL**

EXP2A

![Screenshot 2025-04-07 131048](https://github.com/user-attachments/assets/a3102314-7a70-475c-b91c-b06e955f34ef)

EXP2B

![Screenshot 2025-04-07 131146](https://github.com/user-attachments/assets/04a00c9f-a4c6-43f4-b7e4-6985ec2d5259)


**Timing Diagram**

EXP2A

![Screenshot 2025-04-07 133814](https://github.com/user-attachments/assets/b58209e1-f826-4b4c-9b13-b0130ca1c75b)

EXP2B

![Screenshot 2025-04-07 140751](https://github.com/user-attachments/assets/f42bd041-df47-4265-aedc-d30bc24013ca)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

