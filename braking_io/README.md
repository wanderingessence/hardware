# Purpose
The Braking IO board (generically called Remote IO or RIO boards) are responsible for managing the sensors and actuators on each of the braking trays. Previously, we routed several dozen wire harnesses across the majority of the pod in order to connect to the pressure sensors and solenoids. This board reduces all of that routing into a single power harness, UART + Heartbeat cable and allows for more localized routing to each of the sensors and actuators on the tray. Eventually, there will be 2 of these boards on the pod; one for each braking tray

# Requirements
* Mechanical:
   * Board shall have at least four 4-40 mounting holes
   * Board shall fit in the mechanical enclosure
   * Bonus: Board shall contain at least three fiducals for potential automated assembly
* Connector Interface: 
   * Connectors shall be properly rated for voltage and current
   * Connectors shall have a positive locking feature
   * Connectors shall share a common pinout and be polarized
   * connectors shall be kept to a minimum
   * Bonus: System shall be designed for 1:1 harnesses in order to use off the shelf cable assemblies as much as possible. 
   * Bonus: Harness ID pin shall be added to each connector in order to detect if each cable is properly connected or not. 
* Power:
   * Fusing: Bus input shall be fused to protect against over-current events
   * Telemetry: All rails shall have voltage and current sensing
   * Filtering: Bus voltage shall be filtered
   * Rails: 5V and 3V Rails shall be implemented
* Sensors:
   * Pressure: Pressure telemetry inputs (8x) shall be configurable for both voltage and current output pressure transducers
   * Temperature: Two configurable board mount or external temperature sensors shall provide temperature feedback
* Actuators:
  * Solenoids: 8x solenoid driver circuits shall be implemented
  * Bonus: Use the MPQ6610 instead of a traditional N-MOS driver to save on power
  * Bonus: LEDs on each solenoid
* Watchdog:
  * Board shall have a way to reset all solenoids in case of loss of heartbeat or UART connection from either the microcontroller or the primary flight computer
* MCU:
  * Board shall be capable of sending telemetry, over UART, to the primary flight computer
  * Board shall be capable of receiving commands to actuate different valves, over UART, from the primary flight computer
  
# Info
* Schematic Designers @btobin @rcastle1
* Layout: @btobin
* Need-by-date: 10/1/2019
