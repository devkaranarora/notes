
There are several reasons why bus organization is used in the microprocessor:

1.  Memory access: The bus organization is used for accessing memory by transferring the address of the memory location through the address bus and the data to be stored or retrieved through the data bus. This enables the microprocessor to read and write data to and from memory, which is essential for executing instructions and storing data.
2.  I/O operations: The bus organization is used for performing input/output (I/O) operations by transferring the input/output device address through the address bus and the data to be input or output through the data bus. This enables the microprocessor to communicate with peripheral devices such as keyboards, displays, and sensors.
3.  Interrupt handling: The bus organization is used for interrupt handling, where the microprocessor uses the address bus to fetch the interrupt vector and the data bus to fetch the interrupt service routine. This enables the microprocessor to respond to external events and perform time-critical operations.
4.  DMA operations: The bus organization is used for performing Direct Memory Access (DMA) operations, where the data transfer between the memory and I/O devices takes place without the intervention of the microprocessor. This enables high-speed data transfer between devices and reduces the load on the microprocessor.
5.  Control signal transfer: The bus organization is used for transferring control signals between the microprocessor and other components of the system. This enables the microprocessor to control the operation of devices and coordinate the execution of instructions.

**There are three types of buses.**

-   **Address bus –**

The address bus is a unidirectional bus that is used to carry the memory or I/O device address to which the data is to be transferred. The address bus in the 8085 microprocessor is 16-bit wide.

It is a group of conducting wires which carries address only.Address bus is unidirectional because data flow in one direction, from microprocessor to memory or from microprocessor to Input/output devices (That is, Out of Microprocessor). Length of Address Bus of 8085 microprocessor is 16 Bit (That is, Four Hexadecimal Digits), ranging from 0000 H to FFFF H, (H denotes Hexadecimal). The microprocessor 8085 can transfer maximum 16 bit address which means it can address 65, 536 different memory location. The Length of the address bus determines the amount of memory a system can address.Such as a system with a 32-bit address bus can address 2^32 memory locations.If each memory location holds one byte, the addressable memory space is 4 GB.However, the actual amount of memory that can be accessed is usually much less than this theoretical limit due to chipset and motherboard limitations.

-   **Data bus –**

The data bus is an 8-bit bidirectional bus that is used to transfer data between the microprocessor and other components such as memory and I/O devices. It is used to carry data to or from the memory or input/output devices.

It is a group of conducting wires which carries Data only.Data bus is bidirectional because data flow in both directions, from microprocessor to memory or Input/Output devices and from memory or Input/Output devices to microprocessor. Length of Data Bus of 8085 microprocessor is 8 Bit (That is, two Hexadecimal Digits), ranging from 00 H to FF H. (H denotes Hexadecimal). When it is write operation, the processor will put the data (to be written) on the data bus, when it is read operation, the memory controller will get the data from specific memory block and put it into the data bus. The width of the data bus is directly related to the largest number that the bus can carry, such as an 8 bit bus can represent 2 to the power of 8 unique values, this equates to the number 0 to 255.A 16 bit bus can carry 0 to 65535.

-   **Control bus –**

The control bus is a bidirectional bus that is used to carry control signals between the microprocessor and other components such as memory and I/O devices. It is used to transmit commands to the memory or I/O devices for performing specific operations.

It is a group of conducting wires, which is used to generate timing and control signals to control all the associated peripherals, microprocessor uses control bus to process data, that is what to do with selected memory location. Some control signals are:

Memory read

Memory write

1.  I/O read
2.  I/O Write
3.  Opcode fetch
