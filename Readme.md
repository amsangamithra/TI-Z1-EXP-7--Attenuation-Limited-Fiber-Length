212223060241
# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Aim
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

<img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/28074fe1-e571-4356-bf4c-29cf212c8173" />

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of <img width="54" height="38" alt="image" src="https://github.com/user-attachments/assets/56f53e67-161a-4d53-ba6e-e31a3725ea43" />, corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  

---

## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:

- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB  

---

## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  

---

## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  

2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  

---

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name
 
  ## Tabulation
  <img width="1304" height="1379" alt="image" src="https://github.com/user-attachments/assets/a669a2cc-8194-45b4-8925-902a00669510" />

  ## Attenuation-Limited Fiber Length 2.5GB
  <img width="714" height="377" alt="image" src="https://github.com/user-attachments/assets/877a8ab0-67b6-4059-84ee-9b1135f5e6ac" />
  ## Attenuation-Limited Fiber Length 10GB
  <img width="708" height="374" alt="image" src="https://github.com/user-attachments/assets/bd6e0aa8-15c5-4266-aa44-5d4ac6f9a23e" />
  
  
  ## OUTPUT of 10GB
  
  ## Low Noise:
  <img width="1920" height="962" alt="image" src="https://github.com/user-attachments/assets/cb12ee1c-8395-4d2e-96c7-cfa3225797f6" />
  
  ## High Noise:
 <img width="1920" height="944" alt="image" src="https://github.com/user-attachments/assets/7045f76c-ff38-4b31-9d54-9713184ec306" />

## OUTPUT of 2.5 GB

## Low Noise:

<img width="1920" height="942" alt="image" src="https://github.com/user-attachments/assets/364d961e-daa2-4ea1-8e3a-0b3998a91d26" />

## High Noise:

<img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/cc5ceb26-e6a0-4d6a-af0c-c2dfdd4edd31" />

## Result
Thus the experiment was succesfully completed and output is verified
 

- **Summary Table** for each simulation:
  | Fiber Length (km) | Received Power (dBm) | Q Factor | BER |
  |-------------------|-----------------------|----------|-----|
  

- **Written Summary** of observations and explanations of differences.  
