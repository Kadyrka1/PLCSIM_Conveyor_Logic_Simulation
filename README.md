# PLCSIM_Conveyor_Logic_Simulation
PLCSIM Conveyor Logic Simulation

A PLC-based conveyor belt simulation developed in Siemens TIA Portal using an S7-1200 PLC and S7-PLCSIM. The project demonstrates fundamental industrial automation concepts including start/stop motor control, sensor-based object detection, status indication, and box counting logic. The system uses a latched `%M0.0` internal memory bit (`System_Running`) to maintain conveyor operation after the start button is pressed, while the stop button safely disables the process.

The conveyor motor (`%Q0.0`) operates only when the `System_Running` condition is active. A box sensor (`%I0.2`) detects incoming objects on the conveyor and activates an indicator lamp while simultaneously incrementing a CTU counter to track processed boxes. Additional status lamps visualize conveyor activity and sensor states in real time. The simulation was tested and monitored through PLCSIM watch tables, allowing live interaction with inputs, outputs, and internal PLC memory states.

The project will be extended with HMI integration, timers, and 3D visualization to simulate a complete automated conveyor workflow with real-time monitoring and operator control.


<img width="1536" height="1024" alt="e65812e0-7baf-4ff6-a8fa-5329c1eb810a" src="https://github.com/user-attachments/assets/1fe1384d-009d-4071-b971-c7165e36c970" />


<br><br/>
<img width="1920" height="1080" alt="Screenshot 2026-05-16 185608" src="https://github.com/user-attachments/assets/4075ac79-0e6a-4b5f-bdb9-6f86bcc30bed" />


<br><br/>
A PLC-based conveyor system simulation developed in TIA Portal using S7-PLCSIM. The setup models basic conveyor logic where a sensor detects boxes and controls the conveyor motor accordingly. Integrated with a 3D simulation environment, it visualizes real-time movement of objects on the belt, demonstrating fundamental automation concepts like sensor-actuator interaction and PLC program execution.
