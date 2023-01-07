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
````
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: LOKESH RAHUL V V
RegisterNumber:  22004702

Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
````


Logic symbol & Truthtable
RTL realization

### Output:
### RTL
Half Adder:

![Screenshot_20230107_070029](https://user-images.githubusercontent.com/118423842/211153459-8dc932e6-6b4e-49e8-8756-6422f1b9b0ec.png)

Full Adder:
![Screenshot_20230107_070043](https://user-images.githubusercontent.com/118423842/211153527-2b066993-2bea-473a-84f3-9d4d87d68072.png)

### TIMING DIAGRAM

Half Adder:

![Screenshot_20230107_070056](https://user-images.githubusercontent.com/118423842/211153577-82bbb774-81bc-49e2-81ea-1b7112680da6.png)

Full Adder:

![Screenshot_20230107_070109](https://user-images.githubusercontent.com/118423842/211153592-1bc470ca-6c19-43ea-a81c-a6a9abdcf5e8.png)

### TRUTH TABLE 

Half Adder:

![Screenshot_20230107_070123](https://user-images.githubusercontent.com/118423842/211153607-76a4fec5-d93c-49df-917b-91c99aa53596.png)


Full Adder:

![Screenshot_20230107_070201](https://user-images.githubusercontent.com/118423842/211153617-6ba5736b-40f9-4b7b-a675-787a8a0851c9.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
