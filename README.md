# Triple Bypass Version 2
This is a redesign of the fantastic 3bp from dbElectronics and Tian Feng. The goal of this project was to take the initial design and accommodate all models on one pcb without the need to swap parts. 
It was a team effort between Tian Feng, RetroRGB, and Jose Cruz who did the majorty of the testing. 
Ace, FirebrandX and Mobiusstriptech all were part of the group that helped with the redesign and added various ideas and suggestions that lead to the final product.
The audio adjustment work was done with the help of the mdFourier tool by Artemio Urbina found here - https://github.com/ArtemioUrbina/MDFourier.  
Artemio and Bfbii stayed up many late nights running mdFourier to get the levels to match as close as they could to a model 1 va3 genesis.

# Installation Instructions

Currently I suggest using the Audio installation instructions from the mega amp 2.0
http://www.sega-16.com/forum/showthread.php?31989-Take-your-Genesis-audio-to-the-next-level-The-Mega-Amp-2-0-is-here!

For rgb bypass instructions, please see https://www.retrorgb.com/genesistriplebypass.html for now.


# Not Confirmed Working
The schematic uses the same values as https://github.com/tianfeng33/triple-bypass-Version-2. 
The mechanicals changed to ease installation. The final boards are UNTESTED. Use at your own risk.
# Design Files
The designs are done with Kicad 6.0. The designs were done from scratch and are native to Kicad. 
# Change Log from V2
 - Schematics and Layout redrawn from scratch in Kicad.
 - Multiple layouts created for model specific installs. Model 1 has a separate board. Model 2 and 3 use the same board.
 - Video Low Pass Filter (LPF) is off by default. Solder bridge to enable the filter.
# Model 1 Board
 - Board outline avoids having to trim any plastic or pcb. The RF shield might touch the pins of the MiniDIN9 so it should probably not be reinstalled.
 - Solder location reminders on top of board. Following a guide with pictures is recommended.
 - Board has 5.62K ohm pull up resistors on the RGB lines. These were missing from circuit when the VDP pins are lifted.
 - Board uses audio capacitors. Ceramic capacitors can distort audio. Film capacitors and electrolitic capacitors are used instead. Unknown if the difference will be perceivable.
 - The final revision of Model 1 VA7 is the guts of the early Model 2. Do not install in a VA7 because the resistor values will be wrong. It will not damage it but the sound will be wrong.
# Model 2 and 3 Board
 The 3BP Model 2 is most similar to the original project https://github.com/tianfeng33/triple-bypass-Version-2.
  - Jumpers to set which version Genesis it is being installed in.
  - Jumpers are more clearly labeled on which to solder.
  - Solder location reminders on back of board. Following a guide with pictures is recommended.
  - MiniDIN9 hole pattern matches the connector of the system instead of a CUI-MD-90SM.
  - Board outline changed to avoid the power jack pins. The power jack no longer needs to be flush cut.
  - UNTESTED USE AT OWN RISK
# Model 3 Audio Only
 This is a minimalist board that restores audio levels and 32X audio to a Sega Genesis Model 3. 
  - Only three wires need to be soldered. Video signals are not touched.
  - UNTESTED USE AT OWN RISK