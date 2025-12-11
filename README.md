# Real-Time Audio Filter on FPGA (Basys 3 + Pmod I2S2)

A real-time audio-processing system implemented in Verilog on the Basys 3 FPGA.  
It captures live audio through the Pmod I2S2, applies FIR-based Low-Pass, High-Pass, and Band-Pass filtering, and outputs the processed audio with minimal latency.

---

## Features
- Real-time audio input and output using the I2S protocol  
- Fully synthesizable Verilog RTL design  
- FIR filters for LPF / HPF / BPF  
- Filter selection via Basys 3 switches  

---

## Hardware Used
- Basys 3 FPGA 
- Pmod I2S2 audio module  
- Audio input (phone / laptop)  
- Headphones or speaker  

---

## System Architecture

Audio In → I2S Receiver → FIR Filter → I2S Transmitter → Audio Out

---

##  How It Works

### FIR Filter  
- Implemented as a convolution based arithmetic operation.
- Coefficients loaded from matlab files  
- Supports LPF, HPF, and BPF  

### Filter Selection  
- SW0 → Low-Pass  
- SW1 → High-Pass  
- SW2 → Band-Pass  

---


##  FIR Filter Details
- Coefficients generated using MATLAB/Python  
- Higher-order filters can be added easily  
- Real-time processing with minimal delay  


## ⭐ Acknowledgements
- Digilent documentation  
- DSP and FPGA learning resources  
- Open-source FPGA/Verilog communities
