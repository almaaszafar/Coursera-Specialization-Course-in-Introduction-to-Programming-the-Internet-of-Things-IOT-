#           Introduction to the  Internet of Things and Embedded Systems 
 #  *ALMAAS ZAFAR*
 
   #            EASY CONNECTIONS
    
« Thing »

« Thing » + Computational intelligence = Embedded System

« Thing » + Computational intelligence + Network Connection = IoT

Sensors (Input) -> ADC -> µC (IP+FPGA) -> DAC -> Actuators (Output)
• IP: Intellectual Property core (1 function)
• FPGA: Field Programmable Gate Array (Hardware reconfiguration via RAM – Rewiring)

- General Purpose Processors (Many features)

- Digital Signal Processors (Specific features)
 IC: Integrated Circuit (Small electronic device)


#    Components of Embedded Systems

- Development board (Arduino, Raspberry…)

- Connectors (USB, Ethernet…)

- Inputs (Sensors: Simple / Complex)

- Outputs (Actuators)

- Bread board

#    µC characteristics  

- Datapath Bitwidth

- Input/Output pins

- Performance (Clock rate = Seconds / Cycle)

- Timers (Real time)

- ADC

- DAC

- Low power nodes

- Communication protocols

#  µC components  

- Storage elements (Speed, cost)

- Registers (Stores a single value): Special-purpose registers, General-purpose registers

- Register file REG: a set of registers

- Cache memory:
  - Slower than REG
  - Cheaper than REG
  - Instruction cache + Data cache
  
- Main memory:
  - Slower than cache, CPU
  - Cheaper than cache
  - Not in CPU (Connected via bus)
  
#  Compilation & Interpretation 

 Machine language: Binary (001)
 
• Assembly language: Mnemonics (add r0,r1,r2)

• High language: C, C++,Kotlin,JS....

- Compilation: Translate instructions once before running the code (C, C++)
 -> Translation only once -> Saves time
 
- Interpretation: Translate while code is executed (Python)
-> Translation occurs every execution -> Can adapt to runtime situation

* User <-> Application <-> OS <-> Hardware
* Arduino -> No OS ; Raspberry -> With OS


#   Networking with IOT 

- LAN: Ethernet
* Switch: Smart device that transmits data

* Hub: A dunce device that transmits data (There may be possibility of network collision)

- WAN: Internet
   * Routers: From LAN to WAN
   
- MANET (Mobile Ad Hoc Net): WiFi
   * Access point + Mobile / Wireless devices
   
- Protocols: Rules of communication

- Encapsulation: Separation at different layers
