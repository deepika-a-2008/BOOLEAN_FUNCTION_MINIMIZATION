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
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
 ```

Developed by: Deepika A RegisterNumber:25018166 


**RTL realization**
<img width="1621" height="951" alt="image" src="https://github.com/user-attachments/assets/4fa7285b-562e-414c-ab28-2835e5f3e54c" />
<img width="1534" height="874" alt="image" src="https://github.com/user-attachments/assets/e3a13248-a00c-4482-93e2-cc02876bdbb9" />

**Output:**
**RTL**

<img width="1902" height="543" alt="image" src="https://github.com/user-attachments/assets/ee7d2588-7ff9-44a4-ab64-d2408557901e" />
<img width="1913" height="657" alt="image" src="https://github.com/user-attachments/assets/5243a727-0d70-44ed-9ee3-246f837052c7" />


**Timing Diagram**

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

