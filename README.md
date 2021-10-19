# VSD_PLL
**Documentation of PLL workshop on OSU 180nm by VSD** 

<h2>Table of Contents<h2/> 

 1. PLL Introduction  
 2. Specifications  
 3. EDA Open Source Tools  
 4. Phase Detector: Pre-layout and Post Simulation  
 5. Charge Pump: Pre-layout and Post Simulation  
 6. VCO: Pre-layout and Post Simulation   
 7. MUX Circuit Diagram and Pre-layout Simulation  
 8. PLL Simulation  
 9. Acknowledgements  
 
  
<h2>1. Introduction on PLL-Phase Locked Loop</h2>  
A phased-locked loop or phase lock loop (PLL) is a control system that generates an output signal whose phase is related to the phase of an input signal. There are several different types; the simplest is an electronic circuit consisting of a variable frequency oscillator and a phase detector in a feedback loop. The oscillator generates a periodic signal, and the phase detector compares the phase of that signal with the phase of input periodic signal, adjusting the oscillator to keep the phase matched as shown in Fig 1. 
  
  ****  
  ![image](https://user-images.githubusercontent.com/81102519/137951758-7efa6f0f-5957-4787-b31b-6ec003f7d27e.png)  
   Fig 1: Block Diagram of PLL
  
    
<h2>2. Specifications<h2/>  
   
 
 ![image](https://user-images.githubusercontent.com/81102519/137954609-2c0f9ccf-e24f-48dd-b040-476d323afcb6.png)  
   
 
 ![image](https://user-images.githubusercontent.com/81102519/137954817-91149fab-b972-4aec-9712-3b060f7d12f0.png)
 
 <h2>3. EDA Tools</h2>

1. esim : Esim is a open source EDA tool for circuit design, simulation, analysis, and PCB Design.

2. ngspice : Ngspice is a open source spice simulator for electric and electronic circuit.

3. Magic : Open source layout tool to design VLSI circuits.       

<h2>4. Phase Detector</h2> 
A phase detector is a mixer-like circuit that puts out a signal that is proportional to the phase difference between two input signals of the same frequency.The phase detector produces a series of output pulses whose width is proportional to the phase difference. Passing the pulses through a LPF smoothes them into a proportional DC voltage.
Clock Multiplier: It multiplies frequency of clock signal. It is used in processors for operation.  
   
 **Pre-Layout Simulation**  
   
 ![pfd101](https://user-images.githubusercontent.com/81102519/137957534-cf2540d5-a639-4a28-9daa-5f473baece89.jpg)
   
 
  

 <h2>5. Charge Pump</h2> 
Charge pump is one of the important parts o PLL which converts the phase or frequency difference information into a voltage, used to tune the VCO.  
  
 <h2>6. VCO-Voltage Controlled Oscillator</h2>
It is an electronic oscillator whose oscillation frequency is controlled by a voltage input. VCO can be used for frequency modulation (FM) or phase modulation. For ex: VCOs are used in synthesizers to generate a waveform whose pitch can be adjusted by a voltage determined by a musical keyboard or other input.  
  ![vco](https://user-images.githubusercontent.com/81102519/137951456-00a9f028-8462-4343-88aa-a5eb30fd334e.jpg)
  
  **Pre-Layout Simulation**  
  

**Low-Pass Filter**  
A low-pass filter is a filter that passes signals with a frequency lower than a selected cutoff frequency and attenuates signals with frequencies higher than the cutoff frequency. The exact frequency response of the filter depends on the filter design. So basically a LP  filter is the complement of a high-pass filter.






  
  Pre-Layout Final Circuit Simulation  
  ![FPLL](https://user-images.githubusercontent.com/81102519/137950493-3a231407-0577-475b-8f32-afdea804ae50.jpg)
  ![FPLL101](https://user-images.githubusercontent.com/81102519/137950359-145864ed-3274-4263-b51b-7b422a83679b.jpg)
