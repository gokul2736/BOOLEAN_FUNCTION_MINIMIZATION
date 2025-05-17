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

FUNCTION 1  **K-map**

![Screenshot 2024-12-03 224457](https://github.com/user-attachments/assets/de103be7-f809-4a3d-b63b-43514bd26512)


FUNCTION 2   **K-map**

![Screenshot 2024-12-03 224502](https://github.com/user-attachments/assets/c20052a9-c001-4383-838d-8eedb8b4bb4b)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
FUNCTION 1

module function1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

FUCTION 2

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

FUNCTION 1

![de exp2 function1 ss 3](https://github.com/user-attachments/assets/98cd2d90-86df-4607-ab09-d08254da25d5)

FUNCTION 2

![de exp2a funct2 ss 3](https://github.com/user-attachments/assets/196e311b-aaca-4804-9e2f-2c158a6fd40b)


Developed by: Markandeyan Gokul
Register No: 212224240086

**RTL realization**

**Output:**

**RTL**

FUNCTION 1

![de exp2 function1 ss2](https://github.com/user-attachments/assets/bb201ccf-8ba7-4d19-9f2b-7e1c3fc1d382)

FUNCTION 2

![de exp2a funct2 ss2](https://github.com/user-attachments/assets/0ebd5f2c-2959-424b-9baf-21228cd19880)


**Timing Diagram**

FUNCTION 1

![de exp 2 function1 ss1](https://github.com/user-attachments/assets/a3e15bec-9289-492f-a834-65d5808fc798)

FUMCTION 2

![de exp2a funct2 ss1](https://github.com/user-attachments/assets/6606e101-9a0f-4f8e-a5d3-b4020c995c6d)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

