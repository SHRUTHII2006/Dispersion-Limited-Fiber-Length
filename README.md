# Dispersion-Limited-Fiber-Length
Dispersion Limited Fiber Length
# Objective: 
 
Calculate the dispersion-limited fiber length for a fiber optic transport system that 
employs standard single-mode fiber and a directly-modulated single-mode laser diode 
transmitter. 
 
Simulate the resulting system and verify that it meets performance objective.  
 
# Theory: 
 
The maximum allowable dispersion (or pulse spread) <img width="76" height="52" alt="image" src="https://github.com/user-attachments/assets/52dff457-e7aa-4312-aef4-aa4e234afb47" /> is given in terms of the transmission rate R by the following engineering guideline <img width="192" height="124" alt="image" src="https://github.com/user-attachments/assets/4fcb3de9-6a4a-48db-ba5f-f020a6c85d8b" /> This guideline provides reasonable assurance that there will be no significant inter
symbol interference (ISI) due to pulse spread. 
 
For standard single-mode fiber driven by a directly-modulated laser diode transmitter, the 
pulse spread due to chromatic dispersion is given by
<img width="898" height="694" alt="image" src="https://github.com/user-attachments/assets/5499f4b0-2405-4a5f-b773-ce004a76e850" />
<img width="1300" height="974" alt="image" src="https://github.com/user-attachments/assets/bbd90891-43d6-4a5d-92d2-73ed3e4e57eb" />
# Layout: 
Open up the OptiPerformer file called “Dispersion Limited Fiber.osp”. This layout uses 
the Laser Rate Equations laser diode component with default parameters.  It models a 
directly modulated laser diode based using a standard rate equation model. One of the 
effects of this model is that it generates a signal with a spectral width of about 0.6 nm for 
the default parameters with 2.5 Gb/s, return to zero modulation. 
Within the layout, there are several “Visualizers.” The “Optical Time Domain 
Visualizers” allow the user to the view the simulated signal as a function of time. There is 
one at the output of the laser and one at the end of the fiber.  This allows the user to 
directly observe the changes in the pulses due fiber dispersion. The “Optical Spectrum 
Analyzer” allows the user to view the spectral content of the signal. It this lab it is used to 
verify that the spectral width is about 6 nm. The “BER analyzer” provides calculations of 
the Q factor, the bit error rate (BER) and provides a plot of the eye diagram. 
# Simulation:  
Set the laser power such to achieve a transmitter output power of 0 dBm. The transmitter 
power can be viewed by double clicking the “Output Power Meter Visualizer.” The 
power will read -100 dBm until the first run is made.  
Using the chromatic dispersion factor equation, determine the dispersion of the fiber at 
1550 nm and set the fiber dispersion parameter accordingly. 
Using the equations above, determine the dispersion-limited fiber length. 
<img width="1262" height="1044" alt="image" src="https://github.com/user-attachments/assets/e0b20ca6-42b4-4f1b-ac9a-e4f931a85001" />

<img width="1919" height="1020" alt="Screenshot 2026-05-19 180618" src="https://github.com/user-attachments/assets/09c7b636-79b5-465c-ab76-8078b4fdcd53" />
<img width="1919" height="1018" alt="Screenshot 2026-05-19 180603" src="https://github.com/user-attachments/assets/248f6113-d0a8-4be6-a23f-a5357cd3db8c" />
<img width="1919" height="989" alt="Screenshot 2026-05-19 180518" src="https://github.com/user-attachments/assets/8798af8c-0112-4fa9-8d0f-c32482559baf" />
<img width="1919" height="1019" alt="Screenshot 2026-05-19 180548" src="https://github.com/user-attachments/assets/b8decaeb-5a93-4c4e-9121-5393bd7824c0" />
<img width="1919" height="988" alt="Screenshot 2026-05-19 180533" src="https://github.com/user-attachments/assets/f2e0a830-047e-4266-8fd2-cd5c705f4703" /> 

# Tabulation

<img width="994" height="1600" alt="WhatsApp Image 2026-05-25 at 14 41 34" src="https://github.com/user-attachments/assets/71c37366-e7bd-4986-aead-86125b97779e" />

<img width="1352" height="1600" alt="WhatsApp Image 2026-05-25 at 14 41 34 (1)" src="https://github.com/user-attachments/assets/4214ae6a-a41f-4824-ab37-6f505daf7f9d" />


# Result

The dispersion-limited fiber length for the given optical communication system was found to be approximately 10 km. The simulation results showed acceptable BER performance with a clear eye diagram and minimal intersymbol interference. Hence, the system performance was satisfactory and remained within the allowable dispersion limit.
