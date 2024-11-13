## EXP03-Design-and-Implementation-of-D-Flip-Flop-using-Cadence-EDA-Tools

### Aim:
To design and implement a D flip-flop circuit using Cadence EDA tools, analyze its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

### Tools Required:
  - Personal Computer
  - Cadence Virtuoso Software
### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:

1. Right-click and open the terminal window.
2. Type the following commands and press enter
    - csh
    - source /cadence/install/cshrc
    - virtuoso
    
Procedure for Schematic simulation using Cadence

1) Now two windows must open

    i)virtuoso/command interpreter window ii)”Whats New…”

2) Close the 2nd window
3) Use 1st window i.e virtuoso window(CIW) for further processing.

    - Create a New Library
    - Create Schematic Cell view.
    - Create the Symbol for schematic Cell view.
    - Create the test Cell view.
    - Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
i) Procedure for Creating a New Library:
  - File → New → Library
  - Name the library (e.g., VLSILAB_EXP_3).
  - Choose "Attach to an existing technology library" and click OK.
  - Attach the library to the technology library gpdk045. Click OK.
    
ii) Create Schematic Cell View:
 In the Virtuoso (CIW) window:
  - Go to 1st window i.e virtuoso(CIW)
  - File-New-Cell view
  - Setup the new file form
       + Library: Select the one you a created.
       + Cell : Give the experiment name Ex: Inverter View_Schematic
       + Type: Schematic press OK

   - Add the required components from the libraries and make the connections.
       + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
       + Click on browse. This opens the library browser
       + Now select the appropriate library for components like
       + Gpdk45 ------------------------nmos1v, pmos1v
       + Create Input and Output pins
       + Make the connections by using fixed narrow wire key
       + Click Check and Save button



![WhatsApp Image 2024-10-08 at 16 00 52_01c39360](https://github.com/user-attachments/assets/40a31b50-2d78-42d5-ac18-544c7c52d3a9)


### iii) Creating the Symbol for Schematic Cell View:

   - In the schematic window, execute
       + Create – Cell view – From Cell view
       + The cell view from cell view window appears
       + Check Lib Name, Cell Name, From View name must be schematic Press ok
   - Now Symbol generation form appears. Click Ok If No changes required
   - A new window with with default symbol is created.
   - Edit the symbol if you want to give actual symbol shape else continue.
   - Execute Create-Cell view-from cell view
   - Library Name and Cell Name must be same which you have used for schematic. Press OK
   - Check for the position of pin side.Prss OK
   - Edit for the shape by Create-Shape-Choose required options to edit.

![WhatsApp Image 2024-10-08 at 16 00 46_26d7e3c5](https://github.com/user-attachments/assets/5a5a6614-6594-4a69-b526-b44e7b3c433f)

### iv) Creating the Test Cell View:
- In the CIW window:
  + File → New → Cell view
- In the new file form, set the following:
   + Library: Select the library you created earlier (e.g., VLSILAB_EXP_3).
   + Cell: Name it something different from the schematic cell (e.g., DFlipFlop_test).
   + View: Select "Schematic."
   + Type: Schematic. Press OK.
- Add the required components and make connections, similar to step ii.

![WhatsApp Image 2024-10-08 at 16 00 45_548ac1ff](https://github.com/user-attachments/assets/439eead0-09f1-4ac0-831f-9a8c8e583062)

<br>


### Analog Simulation by SPECTRE:

   - In test cell view window
   - Launch – ADE L(Analog Design Environment)
       + Execute Setup—Simulation/directory/Host A new window opens
       + Set the simulation window to spectre and click ok
       + Execute Analysis – Choose. A window opens.
       + Select the type and set the specifications and press OK
       + Execute Output s—to be plotted – Select on Schematic
       + Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
   - Execute Simulation -- Net list and Run


![WhatsApp Image 2024-10-08 at 16 00 56_bae6e1af](https://github.com/user-attachments/assets/1cb32b56-7dce-42c3-bdb7-9302145bc9b7)

###  For Transient Analysis:
  - In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms for the D and Q signals.

![WhatsApp Image 2024-10-08 at 16 00 53_7dad838d](https://github.com/user-attachments/assets/5c2fcd58-2100-4e8c-953e-e9cd3f1d7d99)

![WhatsApp Image 2024-10-08 at 16 00 55_07660460](https://github.com/user-attachments/assets/ec6081b4-15eb-4cd5-829b-cc71e55e1e79)


### Results:
  + The experiment successfully demonstrated the design and implementation of a D flip-flop using Cadence EDA tools. 
  + The verification through schematic, symbol creation, and simulation highlighted the practical use of Cadence tools for digital circuit design, with the output correctly reflecting the functionality of the D flip-flop.
