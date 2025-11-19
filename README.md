# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable FULL ADDER**
<img width="1335" height="981" alt="image" src="https://github.com/user-attachments/assets/1a085da4-359d-4781-93cd-afccc17122af" />
FULL SUBTRACTOR
<img width="1341" height="968" alt="image" src="https://github.com/user-attachments/assets/828a4510-0ad1-4932-a6bc-67ac9de85724" />

**Procedure**

Write the detailed procedure here

**Program:**

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
DEVELOPED BY:VIGNESH.K
REGISTERNUMBER:25018207
FULL ADDER
```
module exp4a(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^c
assign carry=(a&b)|(b&c)|(c&a);
endmodule
```
FULL  SUBTRACTOR
```
module exp4b(a,b,cin,diff,borr);
input a,b,cin;
output diff,borr;
assign diff=(~a)&c|b&c|(~a)&b;
assign borr=a^b^c;
endmodule
```

**RTL Schematic**
FULL ADDER
<img width="1735" height="846" alt="image" src="https://github.com/user-attachments/assets/bb8ff639-49be-40f6-b869-de1ca3ca171b" />
FULL  SUBTRACTOR
<img width="1708" height="827" alt="image" src="https://github.com/user-attachments/assets/b4103cf3-2236-4070-8aee-962725d3f0b9" />
**Output Timing Waveform**
FULL ADDER
<img width="1919" height="362" alt="image" src="https://github.com/user-attachments/assets/5de2824c-ff6a-40ca-be08-26c3dfc02ec7" />
FULL SUBTRACTOR
<img width="1906" height="335" alt="image" src="https://github.com/user-attachments/assets/d8d031fd-08bf-40a6-8e47-bab7c974d7f4" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



