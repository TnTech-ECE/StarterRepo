# Electrolysis System
## Function of the system
The role of the system is to implement the process necessary for generating the hydrogen and oxygen gases. The system consists of a pre-made electrolytic cell, a pulse inverter, a rectifier, and permanent magnets. The pulse inverter will be the power source of the system, and the rectifier will be used on the output of the pulse inverter to ensure that the polarity of the input power is consistent. The magnets will be used to boost the system's efficiency.

## Constraints
| No. | Constraints                                                                                   | Origin                               |
| --- | --------------------------------------------------------------------------------------------- | ------------------------------------ |
| 1   | The material of the electrolytic cell housing shall not be reactive with Potassium Hydroxide. | Design Constraint                    |
| 2   | The material of the electrolytic cell should be transparent or translucent.                   | Design Constraint                    |
| 3   | The system shall include a pulse generator and permanent magnets to boost efficiency.         | Design Constraint                    |
| 4   | The pulse generator’s output should be rectified.                                             | Design Constraint                    |
| 5   | The electrolysis cell shall have no permanent storage of gases.                               | OSHA Standards 1910.103 and 1910.104 |
| 6   | Pulse inverter must be able to be shut off within two clock cycles by the safety system.      | Design Constraint                    |
| 7   | Safety system must shut off the system when the cell's pressure is at 15 PSI.                 | Design Constraint                    |


<sup>1</sup>
The material of the cell not being reactive with Potassium Hydroxide is essential both for functionality and safety, given that Potassium Hydroxide will be part of the solution housed in the cell.

<sup>2</sup>
This is a preference decided by the team.

<sup>3</sup>
The pulse generator will be the system's power source, and its frequency and amplitude will be manipulated for optimizing efficiency. The magnets will theoretically serve to bias the ions in the solution toward the electrodes in order to increase interaction and boost efficiency.

<sup>4</sup>
The rectification of the pulse generator's output, while not essential to the function of the system as it is being designed, is prefered as it makes possible future development more approachable. The direct purpose of the rectification is that it keeps the location of hydrogen and oxygen gas generation seperate so that, in the future, the gases can more easily be isolated from one another.

<sup>5</sup>
Hydrogen and oxygen gas will not be stored in the cell as pressurized storage of the gases results in a combustible system.

<sup>6</sup>
This will prevent any excessive delays that may be a safety concern.

<sup>7</sup>
While the pressure capacity of the cell being ordered is unknown, 15 PSI was chosen as a limit given the expectation that pressure should not increase by any substantial amount. With this, the system will be shut off when pressure starts to build,  with 15 PSI being chosen as a safe limit where any fault in the system will not be a safety concern, regardless of the cell's capacity.


## Buildable Schematic
![image](/Documentation/Images/Controller_System/Conceptual/Electrolysis_System.jpg)


## Analysis
The electrolysis water machine is sufficient in size for proper functionality. With one, efficiency testing can be done by using optimization (pulse inverter and Neodymium magnets) and using no optimization for comparison. The magnets selected are sufficient, as there are lots of them which allows for better manipulation of the magnetism used on the system. The pulse inverter being used is highly customizable, meaning that amplitude and frequency can be manipulated for doing proper testing and optimization for efficiency. The rectifier selected for the inverter's output is sufficient, being rated for a maximum of 50A and 1 kV, both larger than the current and voltage that the rectifier is anticipated to be exposed to.


## BOM
| Device                                                | Quantity | Price per Unit | Total Cost |
| ----------------------------------------------------- | -------- | -------------- | ---------- |
| Electrolysis Water Machine with Spray-Gun             | 1        | $93.99         | $93.99     |
| TRYMAG Small Magnets 150Pcs, 12x2mm Neodymium Magnets | 1        | $16.19         | $16.19     |
| Pulse Inverter                                        | 1        | NA             | NA         |
| STMicroelectronics PB5010-E3/45                       | 3        | $3.85          | $11.55     |
| Total                                                 |          |                | NA         |