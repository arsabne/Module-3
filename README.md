# Module-3
## MODBUS implementation in STM32F103C8T6 with STM32 official core in Arduino IDE
I am working on my Master Thesis. I would like to implement Modbus RTU protocol using RS485 UART serial communication between four STM32F103C8T6 with STM32 official core in Arduino IDE.

Is there a full-fleged libary for Modbus RTU protocol using RS485 UART serial communication as mentioned in Modicon Modbus Protocol Reference Guide 6 official document? Literally the whole implementation of Modbus RTU protocol using RS485 UART serial communication for both Master and Slave (Start->Address->Function Code->Data->CRC->Stop) .
If so how can I broadcast the message from Master microcontroller to all the slave microcontrollers? I want to implement this in STM32f103C8T6 to send message to all my slave STM32F103C8T6 microcontrollers.

## Working 
i. I should be able to give Inputs or set some limits or something like that from HMI to Master microcontroller.

ii. The limits or inputs or whatever must be set in the Master microcontroller and from Master microntroller all those inputs or limits must be set for Slave microcontrollers as well.

iii. Then the Master microntroller should be able to send the broadcast request or message to all the slave microcontrollers to get all the data's.

iv. Then the Master microcontroller must get all the sensor values or states of the LED's or Motor's or whatever from Master microcontroller itself.

v. Then, all this data's to be stored sepeartely in Master microntroller.

vi. (from iii.) When the Master microntroller has sent the broadcast request or message to all the slave microcontrollers. (same as iv. for slaves) Then all the slave microcontrollers must get all their sensor values or states of the LED's or Motor's or whatever from themself. (same as v. for slaves) And stored sepeartely in them itself.

vii. Then Master microcontroller should send request or message to each slave microcontroller, one after one to get the stored values or states of the LED's or Motor's or whatever from the Slave microcontroller to the Master microcontroller.

viii. Then there must be over all check in the Master microcontroller to check all data is available for HMI.

ix. If something is missing then the Master must get the missing data from itself or from slaves.

x. Then the Master to should send all the data to HMI from Master Microcontroller.

So, basically I will be controlling the whole thing with HMI having my Master microntroller connected to it and all other Slave microcontrollers connected to Master microcontroller.
