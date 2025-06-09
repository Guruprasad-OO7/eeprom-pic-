📟 EEPROM Counter with LCD Display using PIC

This project demonstrates how to use the EEPROM of a PIC microcontroller to store a counter value and display it on an LCD. The counter retains its value even after power off, thanks to EEPROM persistence.

🧰 Hardware Requirements

- PIC Microcontroller (e.g., PIC16F877A)
- 16x2 LCD Display (connected to PORTD and control pins RE0–RE2)
- Power Supply
- MPLAB IDE + Hi-Tech C Compiler

⚙️ Pin Configuration

 RD0–RD7 - LCD Data lines (D0–D7) 
 RE0 - LCD Enable (EN)       
 RE1 - LCD Read/Write (RW)   
 RE2 - LCD Register Select (RS) 

 🧠 Working Logic

- On startup, the code **reads the counter value** stored in EEPROM address `0x00`.
- It **displays the counter** on an LCD.
- The counter **increments from the stored value to 9**, and resets to 0 after reaching 9.
- Each value is **written back to EEPROM**, so the next boot starts from where it left off.
- The LCD shows each number with a small delay before moving to the next.


