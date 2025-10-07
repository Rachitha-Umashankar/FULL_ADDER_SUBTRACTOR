# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus II

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

i)FULL ADDER

![Image](https://github.com/user-attachments/assets/897cde7e-aa20-4c7c-83f3-34237c91554c)

ii)FULL SUBTRACTOR

![SUB](https://github.com/user-attachments/assets/b3f20ca0-68ee-44cf-b140-f01bc97657a9)

**Procedure**

 1. Type the program in Quartus software.
    
 2. Compile and run the program.

 3. Generate the RTL schematic and save the logic diagram.

 4. Create nodes for inputs and outputs to generate the timing diagram.

 5. For different input combinations generate the timing diagram

**Program:**

i)FULL ADDER

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)FULL SUBTRACTOR

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


**RTL Schematic**

i) FULL ADDER

![diagram](https://github.com/user-attachments/assets/072fdb63-029d-437d-8468-7ed1328a40e0)

ii)FULL SUBTRACTOR

![snap](https://github.com/user-attachments/assets/64290ff9-eabe-465c-9493-45b2407fe883)


**Output Timing Waveform**

i)FULL ADDER

![waveform](https://github.com/user-attachments/assets/5c7115f4-c8b4-4ed7-9162-bc1d75c22645)

ii)FULL SUBTRACTOR

![WAVE](https://github.com/user-attachments/assets/323d77f6-e0c8-4ab2-97b7-772a96ae0bf2)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



