### NAME: B KRISHNAKANTH
### Registration no: 212223230109
# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
## Software :
Quartus prime

## Theory
 A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gate.

## Procedure
1. Create a New Project:
   - Open Quartus and create a new project by selecting "File" > "New Project Wizard."
   - Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).
2. Create a New Design File:
   - Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
   - Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

3. Write the Combinational Logic Code:
   - Open the newly created Verilog or VHDL file and write the code for your combinational logic.
     
4. Compile the Project:
   - To compile the project, click on "Processing" > "Start Compilation" in the menu.
   - Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5. Analyze and Fix Errors:*
   - If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
   - Review and fix any issues in your code if necessary.
   - View the RTL diagram.

6.Verification:
   - Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
   - Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
   - Give the Input Combinations according to the Truth Table amd then simulate the Output waveform

## Program:
```
module flipflops(a,b,Y1,Y2,Y3,Y4,Y5,Y6,Y7);
input a,b;
output Y1,Y2,Y3,Y4,Y5,Y6,Y7;
and(Y1,a,b);
or(Y2,a,b);
not(Y3,a);
xor(Y4,a,b);
nand(Y5,a,b);
nor(Y6,a,b);
xnor(Y7,a,b);
endmodule
```


## RTL realization
![exp2_RTL](https://github.com/Krishnakanth23006762/Experiment--02-Implementation-of-combinational-logic-/assets/138849446/041d80b4-5d14-4c1f-aaaa-6a8f4327a6d5)


## Truth Table
![word table ](https://github.com/Krishnakanth23006762/Experiment--02-Implementation-of-combinational-logic-/assets/138849446/7a31cbaf-0c1c-4fc6-be9e-3570ae8eb7d8)

## Output:
![rtl img](https://github.com/Krishnakanth23006762/Experiment--02-Implementation-of-combinational-logic-/assets/138849446/4677cc49-9038-4a4f-a919-6a03c8eb454b)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
