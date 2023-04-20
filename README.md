# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: VARSHA SHARON
RegisterNumber:  212222100058

HALF ADDER

module hadd (a,b,s,c);
input a,b;
output s,c;
xor(s,a,b);
and(c,a,b);
endmodule

FULL ADDER

module fadd (a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor (d,a,b);
xor (s,d,ci);
and (e,d,ci);
and (f,a,b);
or (co,e,f);
endmodule 
```
# Logic symbol & Truthtable
### HALF ADDER

![image](https://user-images.githubusercontent.com/98278161/233407795-b486bc82-8a33-4de5-bfdf-1ce00e7d77ac.png)

![image](https://user-images.githubusercontent.com/98278161/233406400-aa4e9d48-29bd-4f5e-b6bd-054288a2b00a.png)

### FULL ADDER

![image](https://user-images.githubusercontent.com/98278161/233406669-80489602-3de5-478e-b475-e2e86dc8e600.png)

![image](https://user-images.githubusercontent.com/98278161/233406753-44f6ccc5-279f-425f-989c-d7bb1ec2dba9.png)

# Output:
# RTL

### HALF ADDER
![image](https://user-images.githubusercontent.com/98278161/233406844-fe59d360-9dc1-4fb7-8e18-5dc42c147d30.png)

### FULL ADDER
![image](https://user-images.githubusercontent.com/98278161/233406905-e28db123-32ac-4a86-9a88-6fd7142597c7.png)

# TIMING DIAGRAM

### HALF ADDER
![image](https://user-images.githubusercontent.com/98278161/233407074-e9389a28-b80c-4679-90e0-dd042a70ade8.png)

### FULL ADDER
![image](https://user-images.githubusercontent.com/98278161/233407150-0f0ee126-8953-4023-ac9f-5b6bdda773a2.png)

# Result:
Hence, the half adder and full adder are studied and the truth table for different logic gates are verified.
