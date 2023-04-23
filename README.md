# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.Subashini
RegisterNumber:  212222240106
HALF ADDER:
~~~
module halfadder(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

FULL ADDER:

module fulladd(A,B,Ci,S,Co);
input A,B,Ci;
output S,Co;
wire D,E,F;
xor(D,A,B);
xor(S,D,Ci);
and(E,Ci,D);
and(F,A,B);
or(Co,E,F);
endmodule
~~~
*/

Logic symbol & Truthtable
 

### Output:
### RTL realization
RTL realization of Half adder:
![image](https://user-images.githubusercontent.com/119404951/233855801-f40cd1a6-9b30-460a-93a8-530d757404c9.png)
RTL realization of Full adder:

![image](https://user-images.githubusercontent.com/119404951/233855870-0fa9213d-1865-4547-b3da-02eca6639eae.png)




### TIMING DIAGRAM
Half adder
![image](https://user-images.githubusercontent.com/119404951/233855690-d1ea5ca7-2cf2-4303-8b8d-2cd4308ed4b4.png)
Full adder
![image](https://user-images.githubusercontent.com/119404951/233855709-1ec6ef70-1827-4494-a449-95c1a5134d24.png)



### TRUTH TABLE 
Truth table of Half adder:

![image](https://user-images.githubusercontent.com/119404951/233855505-207d9423-fdac-4f0b-bbb0-14e872a6d07b.png)


Truth table of Full adder:
![image](https://user-images.githubusercontent.com/119404951/233855517-452b60eb-7b91-4635-9ad1-ac8acd065cbb.png)



### Result
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
