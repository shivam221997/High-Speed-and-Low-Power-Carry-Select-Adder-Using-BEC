# High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC

## Project Overview
This project presents the design and implementation of a high-speed and low-power Carry Select Adder (CSA) using Binary to Excess-1 Converter (BEC). This implementation is part of the requirements for the Master of Engineering in Microelectronics at the Birla Institute of Technology and Science, Pilani (Hyderabad).

## Introduction
Power consumption is a critical efficiency factor in designing Very Large Scale Integrated (VLSI) circuits. Adders are fundamental components in Arithmetic Logic Units (ALUs) and other parts of processors. This project focuses on optimizing the performance and power efficiency of adders by using a CSA with BEC.

## Adder Circuits
### Carry Select Adder (CSA)
A CSA uses multiple narrow adders to create fast wide adders. It divides the addition problem into smaller groups, allowing for parallel processing.
The CSA consists of two independent units implementing the addition operation in parallel.
When the carry-in is known, the correct sum is selected through a multiplexer (mux).
![m1](https://github.com/shivam221997/High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC/assets/156662255/26d9a642-4b8e-4304-bfd2-5c6a608e49c5)

### Ripple Carry Adder (RCA)
An RCA is a logic circuit where the carry-out of each full adder is the carry-in of the next.
This causes a propagation delay as each carry bit ripples through the stages, impacting the final result.

## Proposed Method
The proposed method replaces the RCA with Binary to Excess-1 Converter (BEC) in the CSA design to reduce propagation delay and power consumption. The main idea is to use BEC instead of RCA with carry-in (Cin) = 1, optimizing area and power.

### 4-bit BEC with 2:1 mux.
![m2](https://github.com/shivam221997/High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC/assets/156662255/f6555bf7-2063-40e7-9c33-7e30a318f083)
   
 ### Implementation of 4 bit BEC
![m3](https://github.com/shivam221997/High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC/assets/156662255/4049430f-46bc-4393-b21e-e6dcba85077a)
  
 ### Block diagram of proposed 16-bit CSA with BEC
![m5](https://github.com/shivam221997/High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC/assets/156662255/ef210b94-6c24-463d-970c-1d7ad6fe52cc)
  
## Implementation
Implementation Using Vivado (Xilinx)
The implementation of the CSA using BEC is performed using Vivado (Xilinx). The design involves the following steps:

### Designing the 4-bit BEC with 2:1 mux.
### Implementing the CSA with RCA and CSA with BEC.
### Comparing the performance in terms of delay, area, and power consumption.

## output RTL-
![m7](https://github.com/shivam221997/High-Speed-and-Low-Power-Carry-Select-Adder-Using-BEC/assets/156662255/a83342a1-8f9e-4944-bae1-b1dcaaa8df4e)


## Results
Delay and Area Evaluation
The proposed 16-bit SQRT CSLA with BEC was evaluated for delay and area.
The use of BEC resulted in a more efficient design with fewer logic gates compared to the conventional CSLA.
## Comparison of Adders
Delay: The delay in the proposed CSA with BEC is significantly lower compared to the conventional CSA.
Power Consumption: The CSA with BEC consumes less power due to reduced propagation delay and fewer logic gates.
Area: The use of BEC reduces the silicon area required for the adder circuit.
## Conclusion
The proposed CSA with BEC is more efficient in terms of power consumption and area compared to the conventional CSA with RCA.
The BEC logic provides significant advantages by using fewer logic gates, eliminating carry propagation, and reducing delay and power consumption.
Future improvements can be made by using parallel prefix adders for further area and delay reduction.
## References
Ch. Daya Sagar, T. Krishna Moorti, “Design of low power flip-flop using MTCMOS Techniques,” International Journal of Computer Application and Information Technology, Vol.1, No.1, July 2012.
Hematha S, Dhawan A, and Kar H, “Multithreshold CMOS Design for low power digital circuits,” TENCON 2008-2008 IEEE Region 10 Conference, pp.1-5, 2008.
K. Roy, S. Mukhopadhyay, and H. Mahmoodi-Meimand, “Leakage current mechanisms and leakage reduction techniques in deepsubmicrometer CMOS circuits,” Proc. IEEE, vol.91, no. 2, pp. 305-327, Feb. 2003.
Pawar Chander, Pokala Santhosh, Prasad Kurhe, “VLSI DESIGN OF FULL SUBTRACTOR USING MULTI-THRESHOLD CMOS TO REDUCE LEAKAGE CURRENT AND GROUND BOUNCE NOISE,” ISSN, Volume-2, Issue-2, 2015.

## Authors
Shivam Kumar (2022H1230198H)
Dikshant Bhatt (2022H1230169H)
Nikhil Devkar (2022H1230166H)
