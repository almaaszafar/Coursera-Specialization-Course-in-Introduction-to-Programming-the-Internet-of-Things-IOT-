#   THE ARDUINO PLATFORM AND C PROGRAMMING
   #   Almaas Zafar


#   ARDUINO PLATFORM

8- bit microcontroller

ATmega328: µP of Arduino

ATmega16U2: µP of USB communication

•IDE: Integrated Development Environment

•Development Board

•Shields

Firmware: Preprogram = Program written already (Unmodifiable code)

Bootloader: Firmware of Arduino

ICSP (In-Circuit Serial Programming): Method to program Bootloader

Schematic: Wiring diagram of a circuit

-> Flash memory: Non volatile memory

-> SRAM memory: Volatile memory (Power off = Bye)

Serial monitor: To communicate with Arduino

Code -> Combine & Transform -> Compile -> Link (+Libraries) -> Hex File Creation

(.hex) -> Upload on Arduino

*avr – gcc #Cross compilation: Creates an executable object file .o that works on

Another machine (avr for ATmega)

Sketch = Program


   #  DIGITAL VS ANALOG
   
   Digital                              Analog
**   Integers                          Continuous
**  0 or 5V                            0 to 5V (0 to 1023)
**  R / W                              R (ADC)
**  0-13 pins                          A0-A5 pin
