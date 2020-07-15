#  THE RASPBERRY PI PLATFORM AND PYTHON PROGRAMMING FOR THE RASPBERRY PI

# ALMAAS ZAFAR 


# ABOUT 

*ARM microprocessor: Broadcom ARMCortex A7

* 40 GPIO Pins (General Purpose Input Output)

* 4 USB Ports (Keyboard, Mouse)

* HDMI Port

* Ethernet Port

* Micro SD Slot (OS)

* ARM design processors and sell its license, they don’t built them – ARM Intellectual Property

ARM Processor Family:
 
  o Classic Processors (ARM)

  o Embedded Processors (Cortex)

  o Application Processors (Cortex)
  
 

| Raspberry pi    | Arduino           |
| ------------- |:-------------:| 
| OS (Libraries, Functions)      | No OS | 
| Faster Processor (1,4GHz)     | Slower Processor (16MHz)     | 
| 64 bit  | 8 bit      |   
| More Memory  |  Less Memory      |  
| Lower I/O  |  Voltage (3,3V)      |  
| SENSIBLE  | Higher I/O Voltage (5V)      | 

*  Text-based interface (console) vs Graphic interface (desktop)

*  NOOBS: New Out Of Box Software  Raspbian (OS Linux-based)

*  raspi-config: tool to setup different options

*  Overclocking: Increase the clock frequency -> Increase the internal voltage level (15% of processor)

     * Quicker execution of instructions (one instruction per clock)
  
     * Signals have shorter time to travel (reduce time over a clock cycle)
  
     * Temperature of device increases -> Shortens device life

#### User application -> /dev/xxx (files associated with hardware device) -> Device driver (connect files to accesses to device access) -> Hardware device

