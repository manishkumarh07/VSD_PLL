# VSD_PLL
**Documentation of PLL workshop on OSU 180nm by VSD** 

**Table of Contents**  
  PLL Introduction  
  Specifications  
  EDA Open Source Tools  
  Phase Detector: Pre-layout and Post Simulation  
  Charge Pump: Pre-layout and Post Simulation  
  MUX Circuit Diagram and Pre-layout Simulation  
  VCO: Pre-layout and Post Simulation  
  PLL Simulation  
  Acknowledgement
  
**Introduction**

**PLL-Phase Locked Loop**  
A phased-locked loop or phase lock loop (PLL) is a control system that generates an output signal whose phase is related to the phase of an input signal. There are several different types; the simplest is an electronic circuit consisting of a variable frequency oscillator and a phase detector in a feedback loop. The oscillator generates a periodic signal, and the phase detector compares the phase of that signal with the phase of input periodic signal, adjusting the oscillator to keep the phase matched.  
  
  **Pre-Layout Simulation**  
  ![pfd_cp BeforeLPF](https://user-images.githubusercontent.com/81102519/137949179-7a0e309f-795a-4e17-83ba-0e50aa7e9ae9.jpg)
      

**Phase Detector**  
A phase detector is a mixer-like circuit that puts out a signal that is proportional to the phase difference between two input signals of the same frequency.The phase detector produces a series of output pulses whose width is proportional to the phase difference. Passing the pulses through a LPF smoothes them into a proportional DC voltage.
Clock Multiplier: It multiplies frequency of clock signal. It is used in processors for operation.  
  


**Low-Pass Filter**  
A low-pass filter is a filter that passes signals with a frequency lower than a selected cutoff frequency and attenuates signals with frequencies higher than the cutoff frequency. The exact frequency response of the filter depends on the filter design. So basically a LP  filter is the complement of a high-pass filter.

**Charge Pump**  
Charge pump is one of the important parts o PLL which converts the phase or frequency difference information into a voltage, used to tune the VCO.

**VCO-Voltage Controlled Oscillator**  
It is an electronic oscillator whose oscillation frequency is controlled by a voltage input. VCO can be used for frequency modulation (FM) or phase modulation. For ex: VCOs are used in synthesizers to generate a waveform whose pitch can be adjusted by a voltage determined by a musical keyboard or other input.  
  ![vco](https://user-images.githubusercontent.com/81102519/137951456-00a9f028-8462-4343-88aa-a5eb30fd334e.jpg)
  
  **Pre-Layout Simulation**  
  

**EDA Tools:**

esim : Developed by IIT Bombay. It is used to create spice netlists.

ngspice : Open source tool for circuit simulator

Magic : Layout editor for designing layouts and generating spice netlists from it.  
  
  Pre-Layout Final Circuit Simulation  
  ![FPLL](https://user-images.githubusercontent.com/81102519/137950493-3a231407-0577-475b-8f32-afdea804ae50.jpg)
  ![FPLL101](https://user-images.githubusercontent.com/81102519/137950359-145864ed-3274-4263-b51b-7b422a83679b.jpg)
