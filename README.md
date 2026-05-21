<img width="1295" height="651" alt="Screenshot 2026-05-21 192940" src="https://github.com/user-attachments/assets/23157be4-61da-4908-8551-fde82ab63c9c" />
<img width="1295" height="651" alt="Screenshot 2026-05-21 192940" src="https://github.com/user-attachments/assets/e1302710-6b08-4a0a-ac7d-a90f05d73dee" />
# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.


**PROGRAM**
Program for flipflops and verify its truth table in quartus using Verilog programming.
## Developed by: Shreenidhi S
## RegisterNumber:212225040410
verilog

module D_FF(D,Clock,reset,Q);
input D,Clock,reset;
output reg Q;
always@(negedge Clock)//use negative edge clock for triggering condition
if(!reset)
Q<=0;
else
Q<=D;
endmodule

**RTL LOGIC FOR FLIPFLOPS**
<img width="1295" height="651" alt="Screenshot 2026-05-21 192940" src="https://github.com/user-attachments/assets/a6da71d4-2840-4b75-a614-7c39434947ce" />



**TIMING DIGRAMS FOR FLIP FLOPS**
<img width="1285" height="664" alt="Screenshot 2026-05-21 192954" src="https://github.com/user-attachments/assets/c00afff1-951f-4aa0-aeca-2af3fc16275d" />



**RESULTS**
Thus the program to implement a D flipflop using verilog and validating their functionality using their functional tables.
