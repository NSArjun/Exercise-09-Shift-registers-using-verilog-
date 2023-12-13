
# Experiment--09-Implementation-of Shift-registers-using-verilog-
### AIM: To implement PISO , PIPO,PISO  using verilog and validating their functionality using their functional tables
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 
Shift registers are basically of 4 types. These are:

Serial In Serial Out shift register
Serial In parallel Out shift register
Parallel In Serial Out shift register
Parallel In parallel Out shift register
Serial-In Serial-Out Shift Register (SISO) –
The shift register, which allows serial input (one bit after the other through a single data line) and produces a serial output is known as Serial-In Serial-Out shift register. Since there is only one output, the data leaves the shift register one bit at a time in a serial pattern, thus the name Serial-In Serial-Out Shift Register.

The logic circuit given below shows a serial-in serial-out shift register. The circuit consists of four D flip-flops which are connected in a serial manner. All these flip-flops are synchronous with each other since the same clock signal is applied to each flip flop.

![image](https://user-images.githubusercontent.com/36288975/172337366-540cc45e-11fe-4cce-9503-560dc704bc7d.png)
FIGURE -01 
erial-In Parallel-Out shift Register (SIPO) –
The shift register, which allows serial input (one bit after the other through a single data line) and produces a parallel output is known as Serial-In Parallel-Out shift register.

The logic circuit given below shows a serial-in-parallel-out shift register. The circuit consists of four D flip-flops which are connected. The clear (CLR) signal is connected in addition to the clock signal to all the 4 flip flops in order to RESET them. The output of the first flip flop is connected to the input of the next flip flop and so on. All these flip-flops are synchronous with each other since the same clock signal is applied to each flip flop.

![image](https://user-images.githubusercontent.com/36288975/172337438-03416c7e-7c9d-4939-ba34-c355b9fc79c5.png)
FIGURE-02
The above circuit is an example of shift right register, taking the serial data input from the left side of the flip flop and producing a parallel output. They are used in communication lines where demultiplexing of a data line into several parallel lines is required because the main use of the SIPO register is to convert serial data into parallel data.
Parallel-In Serial-Out Shift Register (PISO) –
The shift register, which allows parallel input (data is given separately to each flip flop and in a simultaneous manner) and produces a serial output is known as Parallel-In Serial-Out shift register.

The logic circuit given below shows a parallel-in-serial-out shift register. The circuit consists of four D flip-flops which are connected. The clock input is directly connected to all the flip flops but the input data is connected individually to each flip flop through a multiplexer at the input of every flip flop. The output of the previous flip flop and parallel data input are connected to the input of the MUX and the output of MUX is connected to the next flip flop. All these flip-flops are synchronous with each other since the same clock signal is applied to each flip flop.
![image](https://user-images.githubusercontent.com/36288975/172337544-1632407f-1743-4b17-b480-00663d01e59f.png)
FIGURE-03
A Parallel in Serial out (PISO) shift register us used to convert parallel data to serial data.

Parallel-In Parallel-Out Shift Register (PIPO) –
The shift register, which allows parallel input (data is given separately to each flip flop and in a simultaneous manner) and also produces a parallel output is known as Parallel-In parallel-Out shift register.

The logic circuit given below shows a parallel-in-parallel-out shift register. The circuit consists of four D flip-flops which are connected. The clear (CLR) signal and clock signals are connected to all the 4 flip flops. In this type of register, there are no interconnections between the individual flip-flops since no serial shifting of the data is required. Data is given as input separately for each flip flop and in the same way, output also collected individually from each flip flop![image](https://user-images.githubusercontent.com/36288975/172337661-babb1f90-6286-4d14-8cbd-26a380ee085e.png)
FIGURE-04
A Parallel in Parallel out (PIPO) shift register is used as a temporary storage device and like SISO Shift register it acts as a delay element.

### Procedure
Step 1: Module Declaration. module is a keywords defined in Verilog .
Step 2: Input-Output Delecaration. In SIPO,PISO,PIPO registers we use clock as input.
Step 3: Serial-in to Parallel-out (SIPO) - the register is loaded with serial data, one bit at a time, with
the stored data being available at the output in parallel form.
Parallel-in to Serial-out (PISO) - the parallel data is loaded into the register simultaneously and is
shifted out of the register serially one bit at a time under clock control.
Parallel-in to Parallel-out (PIPO) - the parallel data is loaded simultaneously into the register, and
transferred together to their respective outputs by the same clock pulse.
Step 4: Ending module. endmodule is a keywords defined in Verilog.


### PROGRAM 
Program for  Implementation-of Shift-registers-using-verilog-
Developed by: ARJUN N S
RegisterNumber:  212223230020

## PROGRAM:
### SERIAL INPUT PARALLEL OUTPUT:
![SIPO CODE](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/ec25d99b-030f-4028-908d-45b63e8551c7)

### PARALLEL INPUT SERIAL OUTPUT:
![PISO CODE](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/553541b1-9fa5-4aa0-908a-f173c3795f50)
### PARALLEL INPUT PARALLEL OUTPUT:
![PIPO CODE](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/a296592a-551c-4982-9359-b20e66ee873b)


## RTL LOGIC  REGISTERS   
### SERIAL INPUT PARALLEL OUTPUT:
![SIPO RTL](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/7ae56229-3c87-47e2-83e6-25fa1e108d37)
### PARALLEL INPUT SERIAL OUTPUT:
![PISO RTL](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/d4a9ae09-fb78-4547-8e9c-7e1f7bca186d)
### PARALLEL INPUT PARALLEL OUTPUT:
![PIPO RTL](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/ca3a1cf7-e168-44d4-89c1-46ef192c44a9)

## TIMING DIGRAMS FOR SHIFT REGISTERS
### SERIAL INPUT PARALLEL OUTPUT:
![SIPO TIME](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/d758951b-5f84-40e2-9145-3df20a2dd791)


### PARALLEL INPUT SERIAL OUTPUT:
![PISO TIME](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/9a39788b-f5d9-47d4-a067-533031d200bd)


### PARALLEL INPUT PARALLEL OUTPUT:
![PIPO TIME](https://github.com/NSArjun/Exercise-09-Shift-registers-using-verilog-/assets/148233801/d1d7bdd3-381b-4060-b93f-981117c6736b)


### RESULTS:
Implementation of PISO , PIPO, PISO using verilog program is done and its functionality is validated using their functional tables.
 
