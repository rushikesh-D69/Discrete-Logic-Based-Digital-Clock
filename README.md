# Digital Clock using Digital ICs (24-Hour Format)

This repository contains the schematic and design documentation for a fully functional 24-hour digital clock implemented using discrete digital ICs. The clock displays hours, minutes, and seconds on 7-segment displays and includes reset logic for full cycle operation.

WORKING MODEL: https://drive.google.com/file/d/1SXhtJnb3Bu8AmFg-KeR7OFbM0n97bKH2/view?usp=sharing 
![image](https://github.com/user-attachments/assets/d539cc95-36ca-4ffb-9358-e08ec521cad8)

## Project Description

This clock circuit uses a combination of CD4026 counter/display driver ICs, a 555 timer for pulse generation, and various logic components to create a real-time digital clock. The display is in HH:MM:SS format using six 7-segment displays. A reset mechanism is included to return the time to 00:00:00 or enable manual adjustment.

## Features

- Displays time in 24-hour HH:MM:SS format
- Real-time second counting using 1Hz clock pulse from 555 timer
- Six 7-segment displays driven by CD4026 ICs
- Proper carry-over logic between seconds, minutes, and hours
- Reset and manual set buttons included
- Logic implemented using 7411 AND gates and discrete diodes
- Debounced push buttons and stable power management

## Components Used

| Component            | Quantity |
|----------------------|----------|
| CD4026 IC            | 6        |
| 7411 AND Gate IC     | 1        |
| NE555 Timer IC       | 1        |
| MAN74A 7-Segment     | 6        |
| 1N4148 Diodes        | 5        |
| PCB Board            | 1        |
| IC Sockets & Wires   | As required |

## Circuit Overview

- The 555 timer generates a stable 1Hz clock signal.
- CD4026 ICs are used to count and drive each 7-segment display.
- Reset logic is implemented using 7411 AND gates and diodes to reset counters at 60 seconds, 60 minutes, and 24 hours.
- Debouncing capacitors are used with the push buttons.
- A regulated 5V power supply ensures consistent operation.


## Results

The clock operates reliably and accurately, successfully counting and displaying time. All transitions (e.g., from 59 to 00, 23 to 00) function correctly. Challenges such as signal instability and display flicker were addressed through proper wiring, stable power supply, and logic tuning.

## License

This project is intended for educational use and is open for public reference and modification under the MIT License.


