# Rotation-speed-detector
Digital rotational speed detector using IR sensor, 555 timer, CD4040, CD4518 and CD4511 with 7-segment display output
# Digital Rotational Speed Detector using IR Sensor

## Overview
This project implements a **digital rotational speed detection system** using discrete analog and CMOS digital integrated circuits. The system measures the rotational speed of a motor using a **non-contact IR sensor** and displays the result on **two 7-segment displays**.

The design demonstrates fundamental concepts of **signal conditioning, digital counting, timing circuits, and display decoding** without the use of microcontrollers.

---

## Features
• Non-contact rotational speed measurement  
• Uses optical IR sensing  
• Real-time digital display of speed  
• Uses standard CMOS ICs  
• Simple and low-cost hardware design  
• Educational demonstration of analog and digital electronics concepts  

---

## Components Used

| Component | Purpose |
|---------|--------|
| IR Sensor Module | Detect rotational motion |
| IC 741 | Comparator for pulse generation |
| CD4040 | Frequency divider |
| CD4518 | BCD counter |
| CD4511 | BCD to 7-segment decoder |
| NE555 Timer | 1-second timing window |
| 7-Segment Displays | Speed display |
| Resistors & Capacitors | Signal conditioning |

---

## System Working

The system works by converting mechanical rotation into electrical pulses and then processing them digitally.

1. **IR Detection**
   - A rotating disc interrupts or reflects IR light.
   - The IR sensor generates voltage pulses.

2. **Comparator Stage**
   - IC741 converts the analog sensor signal into clean digital pulses.

3. **Frequency Conditioning**
   - CD4040 divides the pulse frequency to stabilize counting.

4. **Counting Stage**
   - CD4518 counts the pulses corresponding to rotations.

5. **Timing Control**
   - A 555 timer generates a 1-second time window for counting.

6. **Display Stage**
   - CD4511 decodes BCD output and drives two 7-segment displays.

The displayed value corresponds to **rotations per second (RPS)**.

---

## Block Diagram

![Block Diagram](images/block-diagram.png)

---

## Methodology Flow

Mechanical Rotation → IR Detection → Comparator → Frequency Divider → Counter → Timing Control → Display

---

## Applications

• Motor speed monitoring  
• Industrial automation systems  
• Robotics  
• Conveyor belt monitoring  
• Educational electronics experiments  

---

## Future Improvements

• Replace IC741 with LM311 comparator  
• Add RPM measurement capability  
• Integrate microcontroller for data logging  
• Use LCD/OLED display  
• Implement direction detection using dual sensors  

---

## Learning Outcomes

This project helps understand:

• Optical sensing techniques  
• Comparator operation  
• Pulse shaping  
• Frequency division  
• Digital counters  
• BCD to 7-segment decoding  
• Time-based measurements  

---

## License

This project is released under the **MIT License**.
