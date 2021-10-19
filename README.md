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
A phased-locked loop or phase lock loop (PLL) is a control system that generates an output signal whose phase is related to the phase of an input signal. There are several different types; the simplest is an electronic circuit consisting of a variable frequency oscillator and a phase detector in a feedback loop. The oscillator generates a periodic signal, and the phase detector compares the phase of that signal with the phase of input periodic signal, adjusting the oscillator to keep the phase matched as shown in Figure 1. 
  
  ****  
  ![image](https://user-images.githubusercontent.com/81102519/137951758-7efa6f0f-5957-4787-b31b-6ec003f7d27e.png)  
   Figure 1: Block Diagram of PLL
  
    
<h2>2. Specifications<h2/>  
   
 
 ![image](https://user-images.githubusercontent.com/81102519/137954609-2c0f9ccf-e24f-48dd-b040-476d323afcb6.png)  
  
 
 ![image](https://user-images.githubusercontent.com/81102519/137954817-91149fab-b972-4aec-9712-3b060f7d12f0.png)
 
 <h2>3. EDA Tools</h2>

1. esim : Esim is a open source EDA tool for circuit design, simulation, analysis, and PCB Design.

2. ngspice : Ngspice is a open source spice simulator for electric and electronic circuit.

3. Magic : Open source layout tool to design VLSI circuits.       

<h2>4. Phase Detector</h2> 
A phase detector is a mixer-like circuit that puts out a signal that is proportional to the phase difference between two input signals of the same frequency.The phase detector produces a series of output pulses whose width is proportional to the phase difference. Passing the pulses through a LPF smoothes them into a proportional DC voltage.
Clock Multiplier: It multiplies frequency of clock signal. It is used in processors for operation. The Post-Layout simulation of Phase detector is shown in figure 4.  
   
 **Post-Layout Simulation**  
   
 ![pfd101](https://user-images.githubusercontent.com/81102519/137957534-cf2540d5-a639-4a28-9daa-5f473baece89.jpg)
   Figure 4: Phase Detector- Post-Layout Simulation
 
  

 <h2>5. Charge Pump</h2> 
Charge pump is one of the important parts o PLL which converts the phase or frequency difference information into a voltage, used to tune the VCO. The layout of charged pump, Pre-layout and Post-Layout Simulation of charge pump is shown in the figure 5.1, 5.2, & 5.3.  
   
 **Charge Pump Layout**  
 
![pfd](https://user-images.githubusercontent.com/81102519/137958678-9d4eb625-cd99-4a7b-846c-c0b1920aad29.jpg)  
   
 Figure 5.1: Layout of Phase-Detector with charge pump
 
 
 **Pre-Layout Simulation**   
 
   ![pfd_cp BeforeLPF](https://user-images.githubusercontent.com/81102519/137958132-7527a723-c390-49e6-98a1-3573e1a0ce1c.jpg)  
     
 Figure 5.2: Charge Pump without Capacitor   
 
 **Post-Layout Simulation**  
   
 ![pfd_cir](https://user-images.githubusercontent.com/81102519/137958896-f38a1403-b12b-44a4-ba1f-21ea7f0bf9f4.jpg)   
   
 Figure 5.3: Charge Pump with Capacitor
  
 <h2>6. VCO-Voltage Controlled Oscillator</h2>
It is an electronic oscillator whose oscillation frequency is controlled by a voltage input. VCO can be used for frequency modulation (FM) or phase modulation. For ex: VCOs are used in synthesizers to generate a waveform whose pitch can be adjusted by a voltage determined by a musical keyboard or other input. The layout of VCO is shown in Figure 6.1, the various values of Pre-layout simulation is shown in Figure 6.2, 6.3, & 6.4 and Post-layout simulation is shown in Figure 6.5.
 
  **VCO Layout**  
 
   ![vco](https://user-images.githubusercontent.com/81102519/137959791-62b30139-0a28-4590-a648-ada300f78c2e.jpg)  

 Figure 6.1: Layout of VCO  
 
  **Pre-Layout Simulation**  
 
 
 ![vco_0 4](https://user-images.githubusercontent.com/81102519/137959895-65e167e6-0f97-4b56-a821-5ab14712e187.jpg)
 Figure 6.2: Simulation of VCO for 0.4V  
   
 ![vco_0 5](https://user-images.githubusercontent.com/81102519/137959903-eb3c27f0-e9cd-4945-9a24-61c9181044eb.jpg)
 Figure 6.3: Simulation of VCO for 0.5V  
  
 ![vco_0 6](https://user-images.githubusercontent.com/81102519/137959905-7ea48040-b8db-4e68-b9c2-8a41776f735d.jpg)
 Figure 6.4: Simulation of VCO for 0.6V  
 
 **Post-Layout Simulation**  
 
 Figure 6.5: Simulation of VCO






  
  Pre-Layout Final Circuit Simulation  
  ![FPLL](https://user-images.githubusercontent.com/81102519/137950493-3a231407-0577-475b-8f32-afdea804ae50.jpg)
  ![FPLL101](https://user-images.githubusercontent.com/81102519/137950359-145864ed-3274-4263-b51b-7b422a83679b.jpg)
