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

**Procedure**

/* write all the steps invloved */
1.Create a new project in Quartus Prime and add a Verilog file.

2.Write the encoder module using dataflow modelling with assign statements for outputs.

3.Compile the design to check for errors.

4.Simulate the design using test vectors from the truth table.

5.Verify outputs and analyze RTL and timing diagrams for correct functionality.

**PROGRAM**


```
module encodder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0 = d1|d3|d5|d7;
assign a1 =d2|d3|d6|d7;
assign a2 =d4|d5|d6|d7;
endmodule
```
**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![318707268-60eebe0b-b007-4c23-a016-6436f6061356](https://github.com/user-attachments/assets/e1cc3a4d-a331-455d-9df1-92f8b869d2ad)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![318707371-451fb2a6-c498-4620-a4cc-fbcc1d7ac99c](https://github.com/user-attachments/assets/31213daf-1949-412c-b360-a2d2dc781d7b)

**RESULTS**

Thus the code is executed successfully.


