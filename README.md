# Morse Code input system (Raspberry Pi Pico Project)

This project was developed as part of a university group assignment (3 members).  
It implements a Morse code input and decoding system using a Raspberry Pi Pico, with input via a button and outputs through a seven-segment display, RGB LEDs, and a buzzer.  

The system allows the user to input letters via short and long button presses (morse code dots and dashes), which are then decoded into letters and displayed on the seven segment display while the morse code is output via the buzzer for auditary confirmation.

The RGB LEDs light up green for a recognised letter and red if not. It will also show red if too long of a gap is left between entering letters or the button is held down for too long. The buzzer plays a short tune if 4 consecutive letters are inputted correctly. 

## File Overview

- morse_code.c → Main program logic

- includes/seven_segment.h → Seven-segment display control

- includes/buzzer.h → Buzzer control

To set up and use, clone the repository and build with the Pico SDK.
On startup, the system displays a welcome message and an 8 flashes on the seven segment display. 
The user can then begin entering morse code letters, correctly entered letters will display in the system. 

## Pin definitions for Pico

Button 1 - GPIO 16

Button 2 - GPIO 14

Buzzer - GPIO 17

RGB LED ~ Red = 13, Green = 12, Blue = 11

Seven segment display ~ GPIO 6-9, 18-20

## Contributors 
Angela Melbourne

Molly Sheppard

Zoe Weston

This project was created for educational purposes.

Coursework set by Dr Joey Lam
