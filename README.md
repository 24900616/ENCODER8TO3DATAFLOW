### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

 ***Truthtable***
 
 ![WhatsApp Image 2024-12-05 at 11 02 43_8c8ec798](https://github.com/user-attachments/assets/008dc1a2-c0e6-47c8-8d0c-c39ff1dd9840)

**Procedure**

1.Type the program in Quartus software. 2.Compile and run the program. 3.Generate
the RTL schematic and save the logic diagram. 4.Create nodes for inputs and outputs to
generate the timing diagram. 5.For different input combinations generate the timing
diagram.

**PROGRAM**

Developed by: Swetha K RegisterNumber: 24900616
```
module enc(Y,A);
input [0:7]Y;
output [2:0]A;
assign A[2]=(Y[4]|Y[5]|Y[6]|Y[7]);
assign A[1]=(Y[2]|Y[3]|Y[6]|Y[7]);
assign A[0]=(Y[1]|Y[3]|Y[5]|Y[7]);
endmodule
```
**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![WhatsApp Image 2024-12-05 at 11 13 45_09c016f9](https://github.com/user-attachments/assets/2969fdb4-2262-49b1-9990-f21e4afc7182)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![WhatsApp Image 2024-12-03 at 13 56 55_709dd1ca](https://github.com/user-attachments/assets/1829724c-7804-4dc4-9fa2-62d8fb1256bd)


**RESULTS**

 Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is verified



