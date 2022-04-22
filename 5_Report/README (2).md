
# Stepper motor
this project is mainly concentrate about the working of stepper motor

# Stepper motor
INTRODUCTION 

Meaning-A stepper motor is an electromechanical system which is transducing an electrical signal into a mechanical
one. It is designed to accomplish a discrete movement (notion of step) and reach a
precise position.

Why to use stepper motor???

Stepper motors do not operate as DC or brushless motors. They have no integrated electronics, no brushes
and can be controlled in open loop. To get a quick idea, stepper motors are very often considered as particular brushless motor that can be controlled without feedback in open loop. Thus, even though stepper motor
may look a bit more difficult to understand technically, they have the advantage of being very simple to control and need no encoder or special driver to monitor the position of the rotor.


When using a stepper motor?

Stepper motors are suitable for applications where compact and robust solutions are required. They develop
their maximum torque at stand-still which makes them naturally suitable to hold a position. The external
commutation ensures that the speed is perfectly constant even if the load varies. Thanks to the absence of
any electronic component, stepper motors run where the hall sensors or encoders of other type of motor
find their limit: high/low temperatures, external noise disturbances, etc.
Compared to a DC motor, a stepper motor is also much easier to use for positioning application as the notion of step enables the user to know the precise position or displacement of the rotor without feeback: it
runs in open loop.
Stepper motors are as a matter of fact frequently used when the following application requirements are
specified:
- Repetitive positioning tasks with high accelerations (i.e. XYZ of machine tools)
- Whenever the settling time must be short and with repeatable discrete positions.
- Whenever open loop (absence of electronics) makes sense (e.g. for noise immunity).
- For back and forth motions.
- Frequent “start/stop” operation.
- Whenever the duty cycle is relatively small. (Time ON << Time OFF)
- Whenever the actual position must be held with high torque.
- Whenever the actual position must be held when no current is applied (thanks to the residualtorque).
- Whenever long life times is required (i.e. using the brushless design).
- Whenever minor speed variation under load are not allowed (peristaltic pumps, XYZ of machinetools)
- For most small consumer electronic devices, such as hard disc drives, ink jet printers, cameras. 

Stepper motors categories 

There are basically three different stepper motor design types on the market:
- The permanent magnet (PM) design
- The variable reluctance design
- The hybrid design.

step angle

The step angle is the basis of the movement of a stepping motor.
the step angle depends on the total number of magnetic poles of the motor.
the step angle is determined by the formula:

Step angle = 360 degrees / N  where N = (NPH x PH)


Stepper Motor Advantages and Disadvantages
Advantages:
1. The rotation angle of the motor is proportional to the input pulse.

2. The motor has full torque at stand still(if the windings are energized)
3. Precise positioning and repeatabilityof movement since good stepper motors have an accuracy of 3 – 5% of a
step and this error is non cumulative from one step to the next.

4. Excellent response to starting/stopping/reversing.

5. Very reliable since there are no contact brushes in the motor. Therefore the life of the motor is simply
dependant on the life of the bearing.

6. The motors response to digital input pulses provides open-loop control, making the motor simpler and less
costly to control.

7. It is possible to achieve very low speed synchronous rotation with a load that is directly coupled to the shaft.

8. A wide range of rotational speeds can be realized as the speed is proportional to the frequency of the inputpulses.

Disadvantages
1. Resonances can occur if not properly controlled.
2. Not easy to operate at extremely high speeds. 




**ULN 2001 driver circuit**


Features
• Seven Darlingtons per package


• Output current 500 mA per driver (600 mA
peak)

• Output voltage 50 V

• Integrated suppression diodes for inductive
loads


• Outputs can be paralleled for higher current


• TTL/CMOS/PMOS/DTL compatible inputs

• Input pins placed opposite to output pins to
simplify layout


**atmega 328 microcontroller**

The Atmel 8-bit AVR RISC-based microcontroller combines 32 KB ISP flash memory with read-while-write capabilities, 1 KB EEPROM, 2 KB SRAM, 23 general-purpose I/O lines, 32 general-purpose working registers, 3 flexible timer/counters with compare modes, internal and external interrupts, serial programmable USART, a byte-oriented 2-wire serial interface, SPI serial port, 6-channel 10-bit A/D converter (8 channels in TQFP and QFN packages), programmable watchdog timer with internal oscillator, and 5 software-selectable power-saving modes. The device operates between 1.8 and 5.5 volts. The device achieves throughput approaching 1 MIPS/MHz


**working**

Stepper motor is a brushless DC motor that divides the full rotation angle of 360° into a number of equal steps.


The motor is rotated by applying a certain sequence of control signals. The speed of rotation can be changed by changing the rate at which the control signals are applied.


Various stepper motors with different step angles and torque ratings are available in the market.

A microcontroller can be used to apply different control signals to the motor to make it rotate according to the need of the application.

For more information about Stepper Motor and how to use it, refer to the topic Stepper Motor in the sensors and modules section.


Here we are going to interface 6 wires Unipolar Stepper Motor with ATmega32 controller.


Only four wires are required to control the stepper motor. 


Two common wires of stepper motor connected to 5V supply.


ULN2003 driver is used to the driving stepper motor.


Note that to know winding coil and their center tap leads measure resistance in between leads. From center leads, we will get half the resistance value of that winding.

**Full step sequence**

Step	 A	B	C	D


  1	   1	0	0	1
  
  2	  1	1	0	0
  
  3  	0	1	1	0
  
  4 	0	0	1	1
 
**Half step sequence**


Step	A	B	C	D


1	  1	0	0	1


2	  1	0	0	0


3	  1	1	0	0


4  	0	1	0	0

5 	0	1	1	0

6 	0	0	1	0

7 	0	0	1	1

8	 0	0	0	1
















