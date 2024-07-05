
## DC-DC BUCK CONVERTER
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
The PWM controller regulates the output voltage by adjusting the duty cycle (D) of the switching signal. The duty cycle is defined as the ratio of the on-time of the switch to the total switching period.
This means the switch is on for 70% of the switching period.
PWM is also used for switching modulation which inturn can be used for demonstration of Discontinuous Conduction Mode
## Results
Recorded the corresponding  waveforms for output voltage, Inductor current and switchin voltages along with the PWM waveform for switching frequency of 20kHz.
Implemented the above converter in MATLAB SIMULINK and recorded the above specified notations .


