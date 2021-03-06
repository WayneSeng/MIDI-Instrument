# MIDI-Instrument
A MIDI project that uses an Arduino Mega stepper motors, floppy drives, and hard drives to create music. The timerone library and digitalWriteFast library is required. An lcd can also be added to respond to CC messages and display text during playback.

## Project Update April 5, 2022:

I am implementing and testing a new version on an ESP32 and custom PCB. Floppy drives are driven with shift registers instead of direct IO. Floppy drives have full ADSR(attack, decay, sustain, release) control. See the `esp32_test.ino` sketch. 

What I have tested:

4 stepper motors  
8 floppy drives(4 per channel)  
2 HDDs  

MIDI CC(controller change) messages:  

12 - Floppy Sustain  
13 - Floppy Decay  
14 - Floppy & Stepper Trill(12 semitones 80ms)  
15 - Floppy Attack  

## Project Update April 15, 2022:

Im currently implementing a sketch based on the L298N H bridge driver and Arduino Uno. I am testing this sketch on a printer scanbed stepper motor. See the `Printer_MIDI.ino` sketch.
