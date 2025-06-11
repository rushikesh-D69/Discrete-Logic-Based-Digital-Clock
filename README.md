# Digital Clock using Digital ICs (24-Hour Format)

This project is a real-life implementation of a **24-hour digital clock** using basic digital ICs. It features hours, minutes, and seconds counters, with reset logic and full real-time functionality.

---

## 🛠 Features
- Displays **hours, minutes, and seconds**
- Operates in **24-hour format**
- Includes a **reset logic** for all counters
- Built using standard **digital ICs** like 7490, 7447, etc.

---

##  Real-Life Implementation
<p align="center">
  <img src="images/real-circuit-photo.jpg" width="400" />
</p>

---

##  Schematic
The schematic for the clock is included in the `schematic` folder.

- [`finished_Circuit.pdf`](./schematic/finished_Circuit.pdf)

---

##  Components Used
- 7490 Decade Counter ICs
- 7447 BCD to 7-Segment Decoder
- 7-Segment Displays
- 555 Timer IC (as clock pulse generator)
- Logic gates for reset logic
- Capacitors, resistors, breadboard/power supply

---

##  Reset Logic
Implements auto-reset at:
- 24:00:00 back to 00:00:00
- Manual reset using external push-button

