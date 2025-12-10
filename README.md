# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)



**PROGRAM**
module ex12(out,clk,rst);

input clk,rst;

output reg [3:0]out;

always @ (posedge clk)

begin

   if(rst)
   
     out<=0;
     
   else 
   
     out <= out-1;
     
end

endmodule



**RTL LOGIC FOR 4 Bit Ripple Counter**

<img width="1920" height="1080" alt="Screenshot 2025-12-10 112858" src="https://github.com/user-attachments/assets/bfa40b9d-94de-40c9-9364-34d119090fd9" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="1920" height="1080" alt="Screenshot 2025-12-10 113013" src="https://github.com/user-attachments/assets/80df2933-a475-40ed-804f-e4c05b71b7ed" />

**RESULTS**

4 Bit Ripple Counter using verilog and validating their functionality using their functional tables is completed successfully.


