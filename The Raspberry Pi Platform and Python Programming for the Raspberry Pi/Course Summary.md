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

### User application -> /dev/xxx (files associated with hardware device) -> Device driver (connect files to accesses to device access) -> Hardware device

*  NOOBS: New Out Of Box Software  Raspbian (OS Linux-based)

*  raspi-config: tool to setup different options

*  Overclocking: Increase the clock frequency -> Increase the internal voltage level (15% of processor)

     * Quicker execution of instructions (one instruction per clock)
  
     * Signals have shorter time to travel (reduce time over a clock cycle)
  
     * Temperature of device increases -> Shortens device life


## LINUX – RASPBIAN 

- Shell: Text-based user interface that executes commands

- Bash (Bourne again shell): Default shell for Raspbian -> LXTerminal (vs Terminal)

- man commandName #Manual of a command

- pwd #Current directory

- cd ( ; arg ; .. ; path) #Change directory

- ls ( ; -l) #Give contents of current directory -> (d:directory,-file) (user/group/other) (rwx:read/write/execute)

- Mkdir #Make directory ; rmdir ( ; -r {if not empty}) #Remove directory

- nano file #Create a nano editor file (sudo apt-get install nano)

- cat ; head ; last ; tail fileName #Print file content

- cp originalName copyName #Copy file

- mv fileName directory #Move file ; mv fileName newFileName #Rename file

- sudo instruction #Switch user account to root account -> Gain the highest permission level

- Processor: Execution of a program; Background processor vs Foreground processor

- ps #Open task monitor ; PID: Process ID ; kill PID #End a processor ; shutdown #Close a processor

- GUI: Graphic User Interface ; File manager: Regular file interface; startx #Start the GUI


