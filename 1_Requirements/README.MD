## Requirements
# Components required for the stepper motor operation
stepper motor

ULN2001 driver circuit

one 10 kilo ohm resistor

one switch 

atmega 328 microcontroller

simulide software (any latest version)

# stepper motor

A stepper motor, also known as step motor or stepping motor, is a brushless DC electric motor that divides a full rotation into a number of equal steps. The motor's position can be commanded to move and hold at one of these steps without any position sensor for feedback (an open-loop controller), as long as the motor is correctly sized to the application in respect to torque and speed.

# Mechanism

Brushed DC motors rotate continuously when DC voltage is applied to their terminals. The stepper motor is known for its property of converting a train of input pulses (typically square waves) into a precisely defined increment in the shaft’s rotational position. Each pulse rotates the shaft through a fixed angle.

Stepper motors effectively have multiple "toothed" electromagnets arranged as a stator around a central rotor, a gear-shaped piece of iron. The electromagnets are energized by an external driver circuit or a micro controller. To make the motor shaft turn, first, one electromagnet is given power, which magnetically attracts the gear's teeth. When the gear's teeth are aligned to the first electromagnet, they are slightly offset from the next electromagnet. This means that when the next electromagnet is turned on and the first is turned off, the gear rotates slightly to align with the next one. From there the process is repeated. Each of those rotations is called a "step", with an integer number of steps making a full rotation. In that way, the motor can be turned by a precise angle.

The circular arrangement of electromagnets is divided into groups, each group called a phase, and there is an equal number of electromagnets per group. The number of groups is chosen by the designer of the stepper motor. The electromagnets of each group are interleaved with the electromagnets of other groups to form a uniform pattern of arrangement. For example, if the stepper motor has two groups identified as A or B, and ten electromagnets in total, then the grouping pattern would be ABABABABAB.

Electromagnets within the same group are all energized together. Because of this, stepper motors with more phases typically have more wires (or leads) to control the motor.


# Stepper motor system
A stepper motor system consists of three basic elements, often combined with some type of user interface (host computer, PLC or dumb terminal):

Indexers


The indexer (or controller) is a microprocessor capable of generating step pulses and direction signals for the driver. In addition, the indexer is typically required to perform many other sophisticated command functions.


Drivers


The driver (or amplifier) converts the indexer command signals into the power necessary to energize the motor windings. There are numerous types of drivers, with different voltage and current ratings and construction technology. Not all drivers are suitable to run all motors, so when designing a motion control system the driver selection process is critical.


Stepper motors


The stepper motor is an electromagnetic device that converts digital pulses into mechanical shaft rotation. Advantages of step motors are low cost, high reliability, high torque at low speeds and a simple, rugged construction that operates in almost any environment. The main disadvantages in using a stepper motor is the resonance effect often exhibited at low speeds and decreasing torque with increasing speed.


# ULN2001 driver circuit


A relay driver circuit is a circuit which can drive, or operate, a relay so that it can function appropriately in a circuit. The driven relay can then operate as a switch in the circuit which can open or close, according to the needs of the circuit and its operation.

# Resistor
A resistor is a passive two-terminal electrical component that implements electrical resistance as a circuit element. In electronic circuits, resistors are used to reduce current flow, adjust signal levels, to divide voltages, bias active elements, and terminate transmission lines, among other uses.

# switch

a device for making and breaking the connection in an electric circuit.

# atmega 328 microcontroller


The Atmel 8-bit AVR RISC-based microcontroller combines 32 KB ISP flash memory with read-while-write capabilities, 1 KB EEPROM, 2 KB SRAM, 23 general-purpose I/O lines, 32 general-purpose working registers, 3 flexible timer/counters with compare modes, internal and external interrupts, serial programmable USART, a byte-oriented 2-wire serial interface, SPI serial port, 6-channel 10-bit A/D converter (8 channels in TQFP and QFN packages), programmable watchdog timer with internal oscillator, and 5 software-selectable power-saving modes. The device operates between 1.8 and 5.5 volts. The device achieves throughput approaching 1 MIPS/MHz.

## simulide software any latest version


