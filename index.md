## Embedded systems and control engineering project selection

---
### Smart framework prototype for air pressure control in agricultural vehicles
[In collaboration with John Deere](https://www.deere.com/en/index.html)

Design and development of a system capable of measuring the tire pressure and adjusting it to a desired value given by the user from a graphical interface in order to adapt the John Deere vehicles to the terrain conditions it has to traverse, and thus maximize its service life.

A multicore STM32 microcontroller is responsible for the control with a real-time operating system (RTOS). The second core of the microcontroller performs a Fourier analysis of the pump vibrations to compensate for measurement errors due to noise. A CAN-based communication protocol recieved a pressure setpoint to activate the pump or valve. The system is also capable of sending the information to a remote server through the MQTT protocol with an ESP32, so that the user can monitor the pressure of the tires.

I mainly contributed to the closed-loop PID control system, the electronics, the design of the valve-pump system, the multicore programming of the microcontroller and the implementation of the RTOS.

<p>
    <img src="images/P1-control-diagram.png?raw=true"/>
    <em>Closed-loop control diagram</em>
</p>
<p>
    <img src="images/P1-schematic.png?raw=true"/>
    <em>Electric diagram of the system</em>
</p>
<p>
    <img src="images/P1-venturi.gif?raw=true"/>
    <em>Flow simulation of the pump-valve system</em>
</p>
<p>
    <img src="images/P1-freq.png?raw=true"/>
    <em>Fourier analysis of the pump vibrations</em>
</p>
<p>
    <img src="images/P1-GUI.png?raw=true"/>
    <em>Graphical user interface</em>
</p>


---
### Gas detection safety system
[Supervised by Intel](https://www.intel.la/content/www/xl/es/homepage.html)

To implement a safety system that focuses on the detection of harmful gases, interconnected sensors that measure different environmental variables are needed. The system activates ventilation fans and an alarm system if the gas concentration is above the permitted limits measured with an MQ3-alcohol and MQ135-CO<sub>2</sub>. The microcontroller used is an ATmega328P, which additionally communicates via Bluetooth with a computer to monitor the system in real time.

<img src="images/P2-diagram.png?raw=true"/>
<img src="images/P2-schematic.png?raw=true"/>

---
### Smart garbage can system

This smart trash monitoring system uses a Raspberry Pi an ultrasonic sensor to determine the percentage of waste accumulated in the can. The data is sent and stored in a MySQL database deployed with XAMPP, and presented on a dashboard for easy and convenient viewing by users. The idea is, if expanded, to have a network of cans to improve the route efficiency of garbage collection services. 

Two types of MQTT protocol inputs were used in Node-Red to receive measurements from the simulation and the physical sensor. Each input went into a separate function to provide the necessary formatting and perform the evaluation of the requirements. The information was filtered and sent via email and Telegram notifications.

<img src="images/P3-dash.png?raw=true"/>
<img src="images/P3-map.png?raw=true"/>
<img src="images/P3-node.png?raw=true"/>
<img src="images/P3-uml.png?raw=true"/>

---
<p style="font-size:11px"></p>