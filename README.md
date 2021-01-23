SIM Cessna 172 - AutoPilot - DIY<BR />

<H1>WORK IN PROGRESS, don't build this for now, NOT TESTED YET</H1>

Build your own autopilot for simulation cockpit cessna 172.<BR />
Format 159x41 mm for 6.25" stack<BR />
Electronics are design with EasyEDA.<BR />
3D parts are design with SolidWorks.<BR />
Parts printed with ANET A8 and CURA 15.04.6

Only electronics, you can choose the microcontroller of your choice, the base design have addtionnal card for Mega2560R3.

For mine i use Mega2560R3 and Mobiflight on MSFS2020--> <a href='https://www.mobiflight.com/en/index.html'>MOBIFLIGHT</a><BR />
For others controllers you need to design the support for the card, or add wires to link them.

<H2>CURA configuration</H2><BR />
With CURA i modified a plugin to add 2 pauses (printing buttons by example) --> <a href='https://github.com/kkr0kk/c172-autopilot/blob/main/Gcode/pauseAtZ.py'>Here</a><BR />
The first pause is set to 0.25mm height and the second is set to 0.45mm height.<BR />
Or you can use gcode directly, with 0.2mm head<BR />
The process for buttons is to start with WHITE PLA for printing text and the printer will go pause, change to PLA BLACK, Drop down the head directly on Z motors by ONE CLICK (so the Z axis return back to 0 but printer think is 0.2mm), purge the color, and resume.<BR />
It will be printing the black layer (fast), and the printer go pause again, Change to PLA CLEAR, purge and resume.<BR />
Now we have perfect buttons with 3 different color.<BR />
