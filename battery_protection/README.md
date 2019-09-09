# Purpose
The Battery Protection Board is responsible for power management on the low voltage system. This includes battery series/parallel configuration, fusing, removing a bad battery from the bus, power distribution to different loads and low voltage dropout. 

# Requirements
* Mechanical
  * Board shall have at least four 4-40 mounting holes
  * Board shall fit in the mechanical enclosure
  * Bonus: Board shall contain at least three fiducials for potential automated assembly
* Connectors
  * Connectors shall be properly rated for voltage and current
  * Connectors shall have a positive locking feature
  * Connectors shall share a common pinout and be polarized
  * Connectors shall be kept to a minimum
  * Bonus: System shall be designed for 1:1 harnesses in order to use off the shelf cable assemblies as much as possible.
  * Bonus: Harness ID pin shall be added to each connector in order to detect if each cable is properly connected or not.
* Power Distribution
  * Configuration: Board shall take in 4 battery inputs (potentially via ring-terminal interface) and connect batteries in 2s2p configuration
    * Note that configuration and number of cells may later change based on pod power budget
  * Configuration: Batteries shall be removable from the bus via power relays. These relays should be normally closed or possibly latching (TBD) in case of multiple failures. If they are latching, they shall be resettable via MCU output and manual push button
  * Dropout: A 20V dropout line shall be used to automatically turn off the system to protect against under voltage damage
  * Fusing: Board shall contain configurable fusing before each load 
  * Power Interface: Boards shall provide interface Molex Microfit connectors for the Remote IO board, primary flight computer board, pump, and 2 spare connectors for additional loads.
* Telemetry
  * Rail: Board shall provide telemetry for voltage and current of each rail
  * Temperature: Board shall provide telemetry for 6x thermistors for board hot-spots and each battery
* Regulation
  * 5V and 3.3V rails shall be present and copied from the Remote IO design
  * A study shall be conducted on each load to determine if 24V buck-boost regulation is required
  * A study shall be conducted on whether any loads require 12V power
* MCU
  * Board shall be capable of sending telemetry, over UART, to the primary flight computer
  * Board shall be capable of receiving commands to actuate different relays, over UART, from the primary flight computer

# Info
* Schematic design: Shelby Riggleman and Ryan Castle
* Layout: TBD
* Need date: 10/1/19
