## DC-DC Buck Converter
A buck converter, also known as a step-down converter, is a type of DC-DC converter that steps down voltage from its input to its output. This report details a hardware implementation of a buck converter with a pulse width modulator (PWM), taking an input of 25V and providing an output of 17.5V with an inductor current of 1A at a switching frequency of 20kHz.

## Components Used
 Inductor (L): Stores energy and helps in smoothing the current.
Capacitor (C): Filters the output to reduce voltage ripple.
Switch (MOSFET): Acts as a high-speed switch controlled by the PWM.
Diode: Provides a path for the inductor current when the switch is off.
PWM Controller: Generates the pulse width modulated signal to control the transistor.
Resistors: Used for sensing and feedback purposes.
## Specifications
Input Voltage (V_in): 25V
Output Voltage (V_out): 17.5V
Inductor Current (I_L): 1A
Switching Frequency (f_s): 20kHz
## Circuit Design
1. Buck Converter Topology
The buck converter consists of the following main components:

Switch (MOSFET): Turned on and off by the PWM signal.
Diode: Provides a freewheeling path for the inductor current when the switch is off.
Inductor: Limits the rate of change of current.
Capacitor: Filters out the voltage ripple in the output.
2. Pulse Width Modulation (PWM)
The PWM controller regulates the output voltage by adjusting the duty cycle (D) of the switching signal. The duty cycle is defined as the ratio of the on-time of the switch to the total switching period. In this design, the switch is on for 70% of the switching period.

PWM Usage: Used for switching modulation, demonstrating Discontinuous Conduction Mode (DCM).
3. Component Soldering
PCB Soldering: Soldered the components on a general-purpose PCB, ensuring proper isolation between the drive circuit ground and the power circuit ground.
4. MOSFET Control
TL494 Module: Integrated the TL494 module for PWM control of the MOSFET, ensuring efficient switching.
5. Voltage Regulation
Reliable Regulation: Achieved reliable voltage regulation across various applications through precise PWM control.
##  Testing and Validation
1. CCM Operation
Continuous Conduction Mode (CCM): Verified the converter's operation in CCM by observing the switch current and diode voltage waveforms.
2. DCM Demonstration
Discontinuous Conduction Mode (DCM): Demonstrated DCM by reducing the switching frequency and observing the corresponding waveforms.
3. Performance Evaluation
 ## Waveform Analysis:
 Recorded and analyzed waveforms to ensure the converter met the specified performance criteria.
## Results and Observations
1. Voltage Conversion:
Successfully converted a 25V input to a stable 17.5V output with an output current of 1A.
2. Mode Control: 
Demonstrated effective control and operation in both CCM and DCM.
3. Precise PWM Control:
The TL494 module provided precise PWM control, ensuring efficient and reliable performance of the buck converter.
## Conclusion
This project effectively showcased the ability to design, implement, and test a DC-DC buck converter using the TL494 module. The experience gained from this project will be valuable for future endeavors in power electronics and control systems.

## Results
1. Waveform Recording: 
Recorded the corresponding waveforms for output voltage, inductor current, switching voltages, and the PWM waveform at a switching frequency of 20kHz.
2. Simulation:
Implemented the converter in MATLAB SIMULINK and recorded the specified observations.
This report provides a comprehensive overview of the design, implementation, and testing of a buck converter, highlighting the key components, specifications, and results.


