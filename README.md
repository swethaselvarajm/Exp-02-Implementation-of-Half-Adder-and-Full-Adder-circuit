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
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SWETHA.S
RegisterNumber:  212222230155
HALF ADDER:
module EX3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule

FULL ADDER:
module EX31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
*/
```

### Output:
half adder:
![Screenshot 2023-09-13 233511](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/7a00d55c-8664-4f6f-beb0-c68cbd2d1938)
full adder:
![image](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/ec586013-7947-414c-907f-89338f82707a)

### RTL:
half adder:
![Screenshot 2023-09-13 233059](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/9ecdde5a-15e4-47b2-b644-9c6d423c197b)
full adder:
![image](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/2d853ee5-6d68-4a11-8e25-f5e87e54adfe)

### TRUTH TABLE :
half adder:
![image](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/a72f4203-4e6c-4289-b474-0412d816202f)
full adder:
![image](https://github.com/swethaselvarajm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119525603/70b3a065-f189-4e19-b1e6-36402c2989bf)

### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
