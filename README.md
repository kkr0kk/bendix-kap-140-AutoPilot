<H1>SIM Cessna 172 - AutoPilot - DIY</H1>

<H1>WORK IN PROGRESS, don't build this for now, NOT TESTED YET</H1>

Build your own autopilot for simulation cockpit cessna 172.<BR />
Format 159x41 mm for 6.25" stack<BR />
Electronics are design with EasyEDA.<BR />
3D parts are design with SolidWorks.<BR />
Parts printed with ANET A8 and CURA 15.04.6

Only electronics, you can choose the microcontroller of your choice, the base design have addtionnal card for Mega2560R3.

For mine i use Mega2560R3 and Mobiflight on MSFS2020--> <a href='https://www.mobiflight.com/en/index.html'>MOBIFLIGHT</a><BR />
For others controllers you need to design the support for the card, or add wires to link them.
<img src='https://github.com/kkr0kk/c172-autopilot/blob/main/images/AP%20-%203D%20view.png?raw=true'></img>
<H2>ELECTRONICS</H2>
<img src='https://github.com/kkr0kk/c172-autopilot/blob/main/images/main%20-%20PCB.png?raw=true'></img>
<H2>3D Printing</H2>
<H3>Materials</H3>
- HEAD : 0.2mm and 0.6mm<BR />
- PLA BLACK, WHITE and CLEAR color<BR />
<H3>CURA  configuration</H3>
With CURA you need plugin PauseAtZ, i modified the plugin to add 2 pauses (printing buttons by example) download and install it--> <a href='https://github.com/kkr0kk/c172-autopilot/blob/main/Gcode/pauseAtZ.py'>Here</a><BR />
<H3>Printing Buttons</H3>
The first pause is set to 0.25mm height and the second is set to 0.45mm height with a config layer height 0.1mm.<BR />
I'm printing buttons with 0.2mm head<BR />
The process for buttons is to start with WHITE PLA for printing text and the printer will go pause, change to PLA BLACK, Drop down the head directly on Z motors by ONE CLICK (so the Z axis return back to 0 but printer think is 0.2mm), purge the color, and resume.<BR />
It will be printing the black layer (fast), and the printer go pause again, Change to PLA CLEAR, purge and resume.<BR />
Now we have perfect buttons with 3 different color.<BR />
<img src='https://github.com/kkr0kk/c172-autopilot/blob/main/images/buttons.png?raw=true'></img>
<H3>Printing Main Parts</H3>
I use a 0.2mm head for the first part, and 0.6mm for the last big part.<BR />
I made 2 STL file, "main.STL" for the first part and "main - second layer printing.STL" for the second part.<BR />
Create 2 gcode files with their parts, parts need to be at the same place (use center platform function).
First Start with 0.2mm head and PLA CLEAR, and when the printer go pause, cancel the print<BR />
Change the head to 0.6mm and PLA BLACK, and start the second part "main - second layer printing.STL".<BR />
GCODE files are on github.<BR />
<H2>SUPPORT for controller</H2>
<H3>Support for Mega2560 pro mini</H3>
<img src='https://github.com/kkr0kk/c172-autopilot/blob/main/images/support_mega2560-pro-mini_PCB.png?raw=true'></img>
<H2>Other Projects</H2>
Build transponder KT76C for Cessna172 -> <a href='https://github.com/kkr0kk/c172-xpndr'>Transponder</a><BR />
