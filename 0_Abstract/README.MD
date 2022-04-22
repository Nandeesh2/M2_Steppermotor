**stepper motor simulation with atmega 328 micro controller in simulide software**


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
