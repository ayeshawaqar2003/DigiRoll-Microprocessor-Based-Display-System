# DigiRoll-Microprocessor-Based-Display-System
A microprocessor-based system using the 8086, 8255A, DIP switches, and seven-segment displays to show specific roll numbers based on input patterns. It demonstrates digital interfacing, programming, and real-time data display through hardware integration.

# Abstract
This project involves using an 8086 microprocessor to display specific roll numbers on seven-segment displays based on dip switch inputs. The system comprises an 8086 microprocessor, 8255A Programmable Peripheral Interface, octal transparent D-type latch, and common anode seven-segment displays. Dip switch patterns are predefined in the code to correspond to each roll number. For example, '0001' displays roll number 85, '0010' for 87, '0100' for 54, and '1000' for 60.

![image](https://github.com/user-attachments/assets/5fba7f34-3e94-448d-a2c8-0a5ccda7f1d8)

# Modules and Interconnections:
## Modules
### 1.	Microprocessor Unit (8086):
o	Central processing unit for executing assembly code.
o	Connected to the data and address buses for communication with peripheral devices and memory.

### 2.	Programmable Peripheral Interface (8255A):
o	Handles input and output operations.
o	Interfaced with the microprocessor to receive DIP switch inputs and send outputs to the seven-segment displays.


###  3.	7-Segment Displays:
o	Used to display numeric values based on the input from the microprocessor.
o	Connected to output ports of the MR8255A/B to show specific numbers corresponding to the DIP switch inputs.

### 4.	DIP Switches:
o	Provide input to the microprocessor to select which number to display.
o	Connected to the input ports of the MR8255A/B.

### 5.	74HC373AD:
An octal transparent latch with 3-state outputs, used to store and isolate data temporarily, such as latching address or data bus information.

### 6.	74HC245:
An octal bus transceiver with 3-state outputs, used for bidirectional data transfer between buses, controlled by direction (DIR) and output enable (OE) signals.


### 7.	74HC244:
An octal buffer/line driver with 3-state outputs, used to buffer and drive data signals, enhancing signal integrity and allowing control over output states.

### 8.	SN74ALS138ANE4 (3-to-8 Line Decoder/Demultiplexer):
o	Decodes the address signals from the microprocessor to select specific devices or memory locations.
o	Facilitates the addressing of multiple peripherals using fewer address lines.

### 9.	Memory (27C16 EPROM):
o	Stores the assembly code and other necessary data for the microprocessor to execute.
o	Interfaced with the microprocessor to provide program instructions.

### 10.	Oscillator (15MHz):
o	Provides the clock signal necessary for the operation of the microprocessor and other timing-dependent components.


### 11.	Buttons:
o	Provide manual input for various control operations.
o	Connected to input ports and used for triggering specific actions in the code.

# Simulation Results:
## Roll Number: 85
 ![image](https://github.com/user-attachments/assets/463e1639-3256-436d-9ce1-5a8686c8b01c)

## Roll Number: 87
 ![image](https://github.com/user-attachments/assets/b0388fbf-9d85-4531-80fb-0e8b86383dd2)





## Roll Number: 54
 ![image](https://github.com/user-attachments/assets/9c862cad-a832-4e73-af83-f599f93e2b15)

## Roll Number: 60
 
![image](https://github.com/user-attachments/assets/4baa8762-b09a-4de7-9d7d-529283a60d23)


# Conclusion
This project demonstrated the use of the 8086 microprocessors to interface with peripheral devices and display outputs based on input from DIP switches. The task involved setting up and configuring ports, writing assembly code, and understanding the workings of the 8255A Programmable Peripheral Interface.
This project enhanced our understanding of microprocessor functionality, peripheral device interfacing, and assembly language programming. Key takeaways include mastering assembly code for the 8086 microprocessors, configuring data and code segments, and interfacing with the 8255A Programmable Peripheral Interface to manage inputs from DIP switches and outputs to seven-segment displays. By applying digital logic, we mapped specific DIP switch inputs to display corresponding roll numbers, developing a truth table to define these relationships. Practical implementation involved integrating hardware components like common anode seven-segment displays and DIP switches with the microprocessor setup, demonstrating real-time application of theoretical knowledge. The successful display of roll numbers based on DIP switch inputs showcased the effectiveness of our approach and the reliability of the microprocessor system designed.



