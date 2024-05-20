# BCD SEGMENT:

# AIM:

 To simulate and synthesis finite state machine using vivado.

# APPARATUS REQUIRED: 

  vivado 2023.2.

# PROCEDURE: 
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

# DIAGRAM:

![image](https://github.com/teja2134/teja2134/assets/161149578/7c305272-d0cc-4f29-acbb-03209a830c42)

# VERILOG CODE:

~~~
module bcd7seg(bcd,seg);

input [3:0] bcd;

output [6:0] seg;

reg [6:0] seg;

always @(bcd)

begin

case (bcd)

    0 : seg = 7'b0000001;
    
    1 : seg = 7'b1001111;
    
    2 : seg = 7'b0010010;
    
    3 : seg = 7'b0000110;
    
    4 : seg = 7'b1001100;
    
    5 : seg = 7'b0100100;
    
    6 : seg = 7'b0100000;
    
    7 : seg = 7'b0001111;
    
    8 : seg = 7'b0000000;
    
    9 : seg = 7'b0000100;
    
    default : seg = 7'b1111111; 

endcase

end

endmodule
~~~

# output:

![image](https://github.com/teja2134/teja2134/assets/161149578/68cb9214-e451-4957-9470-1bc6d17c9b54)

# Result:

Thus,the simulation and synthesis of bcd 7 segment by using vivado has been successfully excecuted and verified.
