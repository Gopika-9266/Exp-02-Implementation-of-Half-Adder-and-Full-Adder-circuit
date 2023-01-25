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
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule


module fulladder(a,b,c,sum,carry);
inputs a,b,c;
outputs sum,carry;
assign sum=((a^b)^c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Gopika.R
RegisterNumber: 22009266
*/
Logic symbol & Truthtable

![half-adder2](https://user-images.githubusercontent.com/122762773/214617065-cba1d22c-bb6f-40f9-9045-26fbdae550c5.png)
![full-adder2](https://user-images.githubusercontent.com/122762773/214617416-2262485f-eedf-456f-b674-7fa074270292.png)


### Output:
### RTL:
![Screenshot (13)](https://user-images.githubusercontent.com/122762773/214617609-f8418557-71a3-479f-a3b8-ec42a29ddba1.png)


![Screenshot (16)](https://user-images.githubusercontent.com/122762773/214617794-8307f2b9-3ef3-454f-bf23-5923f7f9ca47.png)



### TIMING DIAGRAM:

![Screenshot (14)](https://user-images.githubusercontent.com/122762773/214618118-41d8584d-5724-4611-8694-74cbee63608d.png)


![Screenshot (17)](https://user-images.githubusercontent.com/122762773/214618185-ce16d3a3-7e6e-4bb2-8a3c-efd464e4ee7b.png) 

### Result:
     Thus the output for the Half adder and Full adder was successfully done.
