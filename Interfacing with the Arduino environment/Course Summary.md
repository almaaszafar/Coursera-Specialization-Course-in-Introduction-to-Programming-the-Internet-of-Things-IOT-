 # INTERFACING WITH THE ARDUINO
 
   #    ALMAAS ZAFAR


# ELECTRICAL CIRCUITS

• Terminal = Pole / Soldering = Soldering / Short circuit = Court circuit

• Diode:

– Forward Bias :

 • ≥ Threshold: PASS

 • ≤ Threshold: NO PASS

– Revise Bias: NO PASS
 
 • Potentiometer: R1+R2=cte (Top +, Middle Out, Bottom -)
 
 # SENSORS
 

• Resistance ~ -> Voltage ~ -> Arduino pin receives a digital value

Resistive sensors (Resistance)

EXP: Photoresistor

Voltage controlling sensors (Pull Up Path)

EXP: Accelerometer (2D) ; Gyroscope (3D)

#  ACTUATORS

*Sends information to environment

~ On-off actuators (digital)

~ Analog voltage control actuators

* DAC  Pulse Width Modulation PWM

* Duty cycle – AnalogWrite(Pin PWM ~, Value 0 to 255 [0% to 100%])

* Example: 50% – Duty cycle: Half the time 1, Half the time 0 -> Give 2,5V

Buzzer – tone(pin, frequency in Hz, duration in ms) #Generate square wave; Fixed duty

cycle 50% -> notone()


#  EEPROM

EEPROM: Electronically Erasable Programmable Read Only Memory

• Non volatile memory

• Writes a single byte at a time (Similar to flash memory)

• 1k bytes for Arduino

• Masking: Process to store data of 2 bytes (1’s in the bits we interested in and 0’s)

• PS: 0xFF is a mask for 255

* #include<EEPROM.h>

* EEPROM.read(address 1 byte 0->1023)

* EEPROM.write(address, data 1 byte)


#  I2C COMMUNICATION

* Serial protocol -> 1 wire, 1 bit at a time -> Saves pins

* Synchronous protocol -> Shares same clock

-> Master: Who starts the communication

-> Slave: Who receives the communication

• Bit width fixed: 2 bits
– 1 bit for data signal
– 1 bit for clock signal

• 2 Wires:
– SDA: Serial Data
– SCL: Serial Clock

o Transaction:

   o Write

   o Read

-> Transmitter: Places data on the bus

-> Receiver: Read data from the bus
