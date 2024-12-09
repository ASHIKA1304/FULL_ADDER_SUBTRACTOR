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

**Truthtable**

FULL ADDER

![WhatsApp Image 2024-12-09 at 18 44 09_b5340c89](https://github.com/user-attachments/assets/a430a082-9c71-42b1-89c4-56ae319b0f32)

FULL SUBRACTOR

![WhatsApp Image 2024-12-09 at 18 44 41_6317631e](https://github.com/user-attachments/assets/708d892f-5039-4ec3-8d72-dde8f882fbb0)



**Procedure**

1. Type the program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations generate the timing diagram.


**Program:**

 Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
Developed by:ASHIKA TR RegisterNumber:24900481

```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
```

```
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```

**RTL Schematic**

FULL ADDER
![WhatsApp Image 2024-12-09 at 19 09 43_2d6dc2f3](https://github.com/user-attachments/assets/2a4bd80d-b011-42d1-9f67-6e6d3b661977)

FULL SUBRACTOR
![WhatsApp Image 2024-12-09 at 19 13 18_0bd74ead](https://github.com/user-attachments/assets/81ef6688-eed6-46ee-ab68-3ae9ee0efd6e)






**Output Timing Waveform**

FULL ADDER
![WhatsApp Image 2024-12-09 at 19 09 56_95d6a187](https://github.com/user-attachments/assets/ed3dc5c0-14e3-45ab-a4b9-8b87565de6ae)

FULL SUBRACTOR
![WhatsApp Image 2024-12-09 at 19 09 57_b6486187](https://github.com/user-attachments/assets/5edb3507-e2a6-460e-a4f0-b2581309c37d)




**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



