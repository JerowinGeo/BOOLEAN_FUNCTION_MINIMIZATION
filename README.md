# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
Developed by: Jerowin Geo J A
RegisterNumber:212223100016
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule
```

**Logic symbol & Truthtable:**
![image](https://github.com/JerowinGeo/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139744/21393ce6-ed54-467f-9924-8777d6cc9eab)

![image](https://github.com/JerowinGeo/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139744/a9584007-d2ac-4a78-9f26-85bf0a78c5bf)

**RTL realization**
![image](https://github.com/JerowinGeo/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139744/999a034a-713f-41a2-88f0-f2c46110b786)

![image](https://github.com/JerowinGeo/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139744/863f6c15-870c-4cca-bf21-8ef1ed348f18)

**Output:**
![image](https://github.com/JerowinGeo/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139744/3f37ff9e-1be1-44f3-8cd4-b01a270fd186)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

