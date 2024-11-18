## Ex No: 03-Design-and-Implementation-of-D-Flip-Flop-using-Cadence-EDA-Tools

### Aim:

To design and implement a D flip-flop circuit using Cadence EDA tools, analyze its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

### Tools Required:

- Personal Computer
- Cadence Virtuoso Software

### Circuit Diagram:

![385741397-dff9f5b6-aed2-4af9-80d2-55338eb52180](https://github.com/user-attachments/assets/b68d93c8-d0a9-4ca2-a81e-9a88461c3419)


### Schematic Simulation:

PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
	- csh
	- source /cadence/install/cshrc
	- virtuoso

Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”

2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
	
  - Create a New Library
  - Create Schematic Cell view.
  - Create the Symbol for schematic Cell view.
  - Create the test Cell view.
  - Analog simulation by spectre



i)	Procedure for Creating New Library.

- File –New – Library
- Name : Give name for ur library Ex: EXP_3
- Enable Attach to an existing technology library, Click OK
- Attach the library to the technology library gpdk045.Click OK

ii)	Create Schematic Cell view.

- Go to 1st window i.e virtuoso(CIW)
- File-New-Cell view
- Setup the new file form
	 + Library: Select the one you a created.
	 + Cell : Give the experiment name Ex: D_FF_Schematic
	 + Type: Schematic press OK
    
- Add the required components from the libraries and make the connections.
	 + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	+ Click on browse. This opens the library browser
	+ Now select the appropriate library for components like 
	+ Gpdk45 ------------------------nmos1v,  pmos1v
	+ Create Input and Output pins
	+ Make the connections by using fixed narrow wire key
	+ Click Check and Save button



![exp3_schematic](https://github.com/user-attachments/assets/83c21070-552e-4b0c-b50a-562f06a6d2cd)

	

 
iii)	Creating the Symbol for schematic Cell view

- In the schematic window, execute 
	+	Create – Cell view – From Cell view
	+	The cell view from cell view window appears
	+	Check Lib Name, Cell Name, From View name must be schematic Press ok
- Now Symbol generation form appears. Click Ok If No changes required
- A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.


![exp3_symbol](https://github.com/user-attachments/assets/5610c21a-e0fd-4dfc-86e5-3dff3f250c2d)


iv)	Creating the new test cell view

- Go to CIW window, Execute File-New-Cell view
	+ Setup the new file form
	+ Library: Select the one you created Eg.EXP_3
	+ Cell: Cell name must be different from the name used in schematic cell view. Ex: D_FF_test
	+ View: Schematic
	+ Type: Schematic press OK
- Follow the step 3(ii) d to make the required connections


![exp3_sim](https://github.com/user-attachments/assets/2978900c-5a6f-4074-8e69-fcde343adf59)


### Analog simulation by SPECTRE

- In test cell view window
- Launch – ADE L(Analog Design Environment)
	+ Execute Setup—Simulation/directory/Host A new window opens
	+ Set the simulation window to spectre and click ok
	+ Execute Analysis – Choose. A window opens.
	+ Select the type and set the specifications and press OK
	+ Execute Output s—to be plotted – Select on Schematic
	+ Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
- Execute Simulation -- Net list and Run


![exp3_trans1](https://github.com/user-attachments/assets/f3381d32-ad2f-4e52-8430-b566b9b6c968)


### For Transient Analysis Settings and Output

 + In the simulation setup, choose transient analysis.
 + Specify the time range for the analysis (start and stop time).
 + Run the simulation and observe the output waveforms for the D and Q signals.

  
![exp3_trans](https://github.com/user-attachments/assets/a479d79b-48a0-4645-bc29-b590a2d1fb92)



![exp3_out](https://github.com/user-attachments/assets/31e146f7-2bb8-4c78-b7fc-5a747dd956bf)

### Results:

The experiment successfully demonstrated the design and implementation of a D flip-flop using Cadence EDA tools. The verification through schematic, symbol creation, and simulation highlighted the practical use of Cadence tools for digital circuit design, with the output correctly reflecting the functionality of the D flip-flop.









