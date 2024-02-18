directory 

3.2.1 von Neumann system 

3.2.2 Processor Structure 

3.2.3 memory hierarchy 

3.2.4 knowledge points 

3.2.5 system to learn Python 

##  3.2.1 von Neumann system 

Computers are essentially electronic devices that cannot understand human language instructions. In order to enable such electronic devices to perform certain calculations according to human will, scientists have conceived many theories. The most famous of these is the "von Neumann system". In the von Neumann system, computer hardware consists of five parts: arithmetic units, controllers, memory, input devices, and output devices. The data and instructions processed by the computer are represented by binary numbers. The von Neumann system is shown in the following figure: 

![avatar]( 23f3ed19ef30875d76f8a4267ef161fe.png) 

Modern computers are developed on the basis of the von Neumann system, and understanding their components helps to establish a comprehensive understanding of computers. 

(1) Input devices and output devices 

Input and output devices are also known as I/O devices. 

>  I in IO is the first letter of the English word Input, which means input, and O is the first letter of the English word Output, which means output. IO together is input and output. 

Input devices are used to receive user input and transmit it to a computer. Common input devices include the following: 

Mouse, keyboard, camera. 

The output device is the end point device of the computer, which is mainly used to output and display data. The monitor is the most common type of output device. 

(2) arithmetic unit and controller 

The arithmetic unit and the controller form the core of the computer. The CPU in modern computers includes both the arithmetic unit and the controller. The arithmetic unit is used to perform arithmetic calculations and logic operations, and the controller is used to control the various components to work together. 

>  The basic arithmetic operations are addition, subtraction, multiplication and division, and the logical operations are also called Boolean operations. In logical algebra, there are three basic logical operations: and, or, and non. 

(3) Storage 

Memory, as the name suggests, is used to store information in a computer. Memory in a computer can be divided into main memory and external memory according to its function. Main memory is commonly referred to as memory, which is used to store currently active programs and data, with fast read and write speed and small capacity. External memory is used to store programs and data that need to be stored for a long time, with slow read and write speed and large capacity. The main memory cannot store data permanently. After the machine is powered off, all the information in the main memory will be lost. For persistent storage, data needs to be written to external memory. Common external memory devices: 

>  Hard disks, tapes, USB flash drives and CDs 

##  3.2.2 Processor Structure 

The processor in a computer is commonly referred to as the CPU. CPU is the abbreviation of Central Processing Unit, which means Central Processing Unit, which is the computing core and control core of the computer. The CPU can be logically divided into three modules: Control Unit, Operation Unit and Storage Unit. Each unit is connected by an internal bus. The logic structure of the CPU is shown in the following figure: 

![avatar]( 809c64b82fcb6b4941655384ad034ca5.png) 

(1) Control Unit 

The Control Unit is the command and control center of the CPU, which is mainly composed of a program counter PC, an instruction register IR, an instruction decoder ID, and an operation controller OC. 

![avatar]( e93f1b30b3f44bdc0836f9adb0a07fcf.png) 

The program counter contains the address of the instruction to be executed. When the instruction is fetched by the CPU, the storage address in the program counter is incremented, and the program counter points to the next instruction in the instruction sequence. 

The core task of the CPU is to execute the instructions in the program, and the instructions and data in the program are stored in memory. The program counter initially points to

For the first instruction in the sequence, the CPU obtains the address of the first instruction from the program counter, and then reads the instruction from the memory and executes it.

When the CPU executes an instruction, it synchronously modifies the contents of the program counter so that the program counter always points to the next instruction to be executed.

Computer programs are executed in this manner.

After the CPU fetches the instruction from memory, it places it in the instruction register, and then decodes the instruction through the decoder to determine what operation to perform. 

Program instruction is composed of operation code and address code. It decodes the instruction, that is, extracts the operation code and address code in the instruction.

The opcode indicates which operation to perform, and the address code indicates the address where the operand is stored.

For example, the addition operation 1 + 2 has operands 1 and 2, and the opcode indicates that an addition operation is required.

After the instruction is decoded, the operation controller generates various operation control signals according to the operation code and timing signal of the instruction, thus completing the control of the instruction acquisition and execution of the instruction. 

(2) Storage unit 

It is composed of the on-chip cache and register group in the CPU, which is a unit for the CPU to temporarily store data, which stores data waiting to be processed or has been processed. 

(3) Operating unit 

The core of an arithmetic unit used to perform arithmetic and logic operations. 

##  3.2.3 memory hierarchy 

Registers are the basic storage unit of the CPU, and the CPU takes much less time to access registers than memory access. To reduce the number of times instructions and data are read from memory, a cache is introduced between the CPU and memory. Similarly, memory reads and writes much faster than disk reads and writes. To reduce the number of disk reads and writes, read and write buffers are introduced into computer memory. These memories are organized into a pyramid-shaped hierarchy in the logical structure of the computer according to their access speed and capacity: 

![avatar]( 05e7c3bd40fa40cf7f13a58f3b93a067.png) 

It can be seen from the figure that the access speed of the register is the fastest, and the access speed of the external memory is the slowest. From the perspective of the size of the capacity, the storage capacity of the register is the smallest, while the storage capacity of the external memory is the largest. 

The hierarchical structure of memory shows that although fast storage devices are fast, their capacity is small, and slow storage devices are slow to read and write.

But the storage capacity is large. According to this idea of memory hierarchy, fast storage devices can be used as caches for slow storage devices,

For example, the cache is used as a cache for memory, and the memory is used as a cache for disk.

How to use caching to improve program performance is a core technology that programmers must master, and will be explained in detail in subsequent chapters.

##  3.2.4 knowledge points 

>  (1) Computers are essentially electronic devices that cannot understand human language commands

(2) In the von Neumann system, computer hardware consists of five parts: arithmetic unit, controller, memory, input device, and output device.

(3) Main memory is commonly referred to as memory, which is used to store currently active programs and data, with fast read and write speed and small capacity. External memory is used to store programs and data that need to be stored for a long time, with slow read and write speed and large capacity.

(4) The processor in a computer is commonly referred to as the CPU. CPU is the abbreviation of Central Processing Unit, which means Central Processing Unit, which is the computing core and control core of the computer. The CPU can be logically divided into three modules: Control Unit, Operation Unit and Storage Unit. 

##  3.2.5 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

