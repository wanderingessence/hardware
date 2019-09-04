# Silego Designs
See https://www.dialog-semiconductor.com/gpio-expander 

## Silego Basics
These chips are configurable mixed-signal devices that allow the user to connect various gates, LUTs, delays, comparators, etc. to create unique, custom hardware logic with fewer external components and rapid iteration. These are pretty neat chips. 

To get started, download GreenPAK Designer https://www.dialog-semiconductor.com/greenpak-designer-software and open a sample .gp* project and check out a reference design

We also have a development and programming board that allows us to test out the circuit in the real-world before committing to a design. If you've taken ECE 352 or ECE 551, you know how important it is to simulate and test your programmable hardware before committing. With an un-programmed part, you can simulate and update your image as much as you'd like, but as soon as you flash the Non-Volatile Memory, that chip cannot be re-programmed. We have a limited amount of components, so we want to make sure we are confident in our design before burning an IC, but know we have the flexibility to adjust even after PCBs have gone out to fabrication or assembly. 
