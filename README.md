# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit, leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.

Identity Law A ⋅ 1 = A, A + 0 = A 
Null Law A ⋅ 0 = 0, A + 1 = 1 
Idempotent Law A ⋅ A = A, A + A = A
Complement Law A ⋅ A′ = 0, A + A' = 1 
Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C 
De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′ 
Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A 
Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
Commutative law A B = B A,A + B = B + A

**Logic Diagram**

identity law:

   ![identity law](https://github.com/user-attachments/assets/a25972c9-10bf-4da0-9acf-e2d53489b804)

null law:

   ![annulment law](https://github.com/user-attachments/assets/7c4ee8df-b780-4726-9bb7-5f700f417d72)

idempotent law:
     
   ![idempotent law](https://github.com/user-attachments/assets/ebfff5ce-5126-41e4-9ba7-ac15af64e9dd)


complement law:

   ![complement law](https://github.com/user-attachments/assets/3326e01a-ab19-4ffb-87d1-7ba5ca220f14)

distributive law:

   ![distributive law](https://github.com/user-attachments/assets/b0fbc701-e203-4f0d-9784-6915de45f750)

De Morgan's law:

   ![de morgan law](https://github.com/user-attachments/assets/de09ab6b-7055-468e-a8ef-35388dc43589)

Absorption law:

   ![absorbtion law](https://github.com/user-attachments/assets/61d19f8e-8c46-4593-a2da-a1afae3a68da)

Associative law:

   ![assosiative law](https://github.com/user-attachments/assets/7e4b6d42-8632-4d78-bcb1-1db4db098086)

Commutative law:

 ![commutative law](https://github.com/user-attachments/assets/1415f82f-25ac-43c0-9d4a-97644a9267f2)

 
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


Developed by : Monish R
Register Number : 25017815

**Output:**
1)

 ![output 1](https://github.com/user-attachments/assets/efc9cd57-b3f3-4414-aa43-60fbe8fe6f93)

2)
 ![output 2](https://github.com/user-attachments/assets/2b03ccc3-498d-488e-bba6-e0b8bf309246)



**Timing Diagram**

1)
  ![timing diagram 1](https://github.com/user-attachments/assets/53fc8052-1052-4111-bb1b-c2228fb6a402)

2)
    ![timing diagram 2](https://github.com/user-attachments/assets/8561c073-9218-49d1-a52b-5c9be5b5a93d)


**Result:**

Thus the given logic functions are implemented  and their operations are verified using Verilog programming.

