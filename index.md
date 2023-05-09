## Embedded systems and control engineering project selection

---

### Smart framework for air pressure control in agricultural vehicles

[In collaboration with John Deere](https://www.deere.com/en/index.html)

Design and development of a system capable of measuring the tire pressure and adjusting it to a desired value given by the user from a graphical interface in order to adapt the John Deere vehicles to the terrain conditions it has to traverse, and thus maximize its service life. This is achieved through the implementation of a closed-loop PID control system inside a STM32 microcontroller that receives through the CAN protocol the information from the reference and sends the corresponding signal to activate the pump or valve to make the pressure adjustment. To compensate for measurement errors due to noise, an inertial measurement unit (IMU) was added to analyze pump vibrations by means of a Fourier analysis performed on the secondary core of said microcontroller. The system is also capable of sending the information to a remote server through the MQTT protocol with an ESP32, so that the user can monitor the pressure of the tires in real time.

<img src="images/P1-control-diagram.png?raw=true"/>
<img src="images/P1-schematic.png?raw=true"/>
<img src="images/P1-3Dmodel.png?raw=true"/>

---
[Project 2 Title](/pdf/sample_presentation.pdf)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---
[Project 3 Title](http://example.com/)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---

### Category Name 2

- [Project 1 Title](http://example.com/)
- [Project 2 Title](http://example.com/)
- [Project 3 Title](http://example.com/)
- [Project 4 Title](http://example.com/)
- [Project 5 Title](http://example.com/)

---




---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
