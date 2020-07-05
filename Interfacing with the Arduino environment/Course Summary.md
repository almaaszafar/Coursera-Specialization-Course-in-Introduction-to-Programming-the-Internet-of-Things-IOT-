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

`EXP: Buzzer – tone(pin, frequency in Hz, duration in ms) #Generate square wave; Fixed duty

cycle 50% -> notone()
