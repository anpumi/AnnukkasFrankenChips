# FunGuy
I’ve had this handmade blown-glass mushroom lamp for about a year.
The glass is gorgeous, but the electronics weren’t. It came with a white plastic battery compartment that offered three functions: On, Off, 6-hour timer.
I wanted it to become part of my Home Assistant setup instead of another battery-powered decoration.

### This repo documents the project as it happened, rather than how I wish it had happened. Therefore, if you're planning on building your own version, please read the Lessons Learned section below first. It'll probably save you time and materials.

## Architecture
<img width="300" height="451" alt="architecture drawio" src="https://github.com/user-attachments/assets/39ff01aa-470c-4de2-8eb0-f686be188183" />

## Features
- ESPHome
- Home Assistant integration
- PWM dimming
- Custom 3D printed parts
- Custom lighting effects running directly on the ESP32

## Hardware
- Waveshare ESP32-C3 Zero
- IRLZ34N logic-level MOSFET
- 5 V USB power
- Existing warm white LED seed light string
- Original mushroom blown glass lamp

## Photos
- [Photos](https://github.com/anpumi/AnnukkasFrankenChips/tree/main/FunGuy/Photos)

## Wiring diagram
- Coming soon

## Build notes
- Coming soon

## Lessons learned
- https://github.com/anpumi/AnnukkasFrankenChips/blob/main/FunGuy/Photos/09-v1_oops.png
- The perfboard was a few millimeters too large to fit inside the printed base.
- Slot design is not ideal for threading the JST connector through.
- The first printed revision has a 2mm gap between the base and the lid because I didn't take into account the thickness of the mating wall. Fixing for v2.

## Version 2 notes
- Replace the original LED seed light string with individually addressable WS2811 clear wire seed pixel string.
    - 5V, 10cm pitch, 20 LEDs/2 meter length.
- Possibly add a capacitive touch sensor to the side of the base.
- Improve base CAD design.

## ToDo
- [ ] Link to Waveshare ESP32-C3 docs.
- [ ] Create wiring diagram in KiCad.
- [ ] Write build notes.
- [ ] Increase base dimensions to accomodate a 40x60 perfboard.
- [ ] Redesign connector routing.
- [ ] Fix Lid height.
- [ ] Add mounting posts for the PCB.
- [ ] Improve/add cable strain.
