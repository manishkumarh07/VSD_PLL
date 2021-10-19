# VSD_PLL
Documentation of PLL workshop on OSU 180nm by VSD 

**Table of Contents**  
  "*" PLL Introduction  
  Specifications  
  EDA Open Source Tools  
  Phase Detector: Pre-layout and Post Simulation  
  Charge Pump: Pre-layout and Post Simulation  
  MUX Circuit Diagram and Pre-layout Simulation  
  VCO: Pre-layout and Post Simulation  
  PLL Simulation
  
**Introduction**

PLL-Phase Locked Loop
A phased-locked loop or phase lock loop (PLL) is a control system that generates an output signal whose phase is related to the phase of an input signal. There are several different types; the simplest is an electronic circuit consisting of a variable frequency oscillator and a phase detector in a feedback loop. The oscillator generates a periodic signal, and the phase detector compares the phase of that signal with the phase of input periodic signal, adjusting the oscillator to keep the phase matched.


Phase Detector
A phase detector is a mixer-like circuit that puts out a signal that is proportional to the phase difference between two input signals of the same frequency.The phase detector produces a series of output pulses whose width is proportional to the phase difference. Passing the pulses through a LPF smoothes them into a proportional DC voltage.
Clock Multiplier: It multiplies frequency of clock signal. It is used in processors for operation.

Low-Pass Filter
A low-pass filter is a filter that passes signals with a frequency lower than a selected cutoff frequency and attenuates signals with frequencies higher than the cutoff frequency. The exact frequency response of the filter depends on the filter design. So basically a LP  filter is the complement of a high-pass filter.



**EDA Tools:**

esim : Developed by IIT Bombay. It is used to create spice netlists.

ngspice : Open source tool for circuit simulator

Magic : Layout editor for designing layouts and generating spice netlists from it.

![ALT](C:\Users\Manish\Pictures\VSD/ckt.jpg?raw=true)
![ckt](https://user-images.githubusercontent.com/81102519/137939494-f6f207b7-bfcf-4f8e-aa49-dcefef270d07.jpg)
