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
   
  Integers             |             Continuous

  0 or 5V              |              0 to 5V (0 to 1023)

  R / W                |              R (ADC)

  0-13 pins            |              A0-A5 pin
  
  
  #   IDE 
  
void setup()  #Initialization (Executed 1 time)

void loop()   #While power is on, loop

pinMode(pin,MODE)   #Setup, MODE=INPUT; OUTPUT ; INPUT_PULLUP

digitalRead(pin)    #returns 0 or 1

digitalWrite(pin,VALUE)   #VALUE=HIGH; LOW / 0;1

analogRead(analogPin)   #returns 0 to 1023 (integers) -> 0 to 5V

 INPUT_PULLUP:  INPUT + Reverse polarity
 
 
 #  DEBUGGING
 
*- Controllability: Inputs / Internal memory

*- Observability: Outputs / Internal memory

    ->  Testing & Debugging

*-Run control of the forget (stop)               } Debugging

*- Real time monitoring of target execution      } Debugging

*- Timing & functional accuracy                  } Debugging

*-> Remote debugger (debug monitor, maintains communication link #break;) *-> Software

*-> Embedded debug interface (in processor) *-> Hardware

*-> Serial protocols (communication protocol between devices to debug with in Arduino, UART)
 
