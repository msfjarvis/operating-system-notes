# Role of Operating System

When the power to a computer is turned on, the first program that runs is usually a set of instructions kept in the computer's read-only memory (ROM), that examines the system hardware to make sure everything is functioning properly.

The POST (Power On Self Test) checks the CPU, memory, and basic I/O systems for errors and stores the result in a special memory location.

Once POST successfully completes, the software that is loaded in ROM (sometimes referred to as firmware) will begin to activate the computer's disk drive(s).

In most modern computers, when the computer activates the hard disk drive (HDD) the first piece of system program it finds is the bootstrap loader.

The bootstrap loader (BSL) is a small program that has a single function -- it loads the Operating System (OS) into memory and allows it to begin operations. In its most basic form, the BSL sets up the small drive(s) programs that interface with and control the various hardware subsystems of the program. It sets up the division of memory that holds the OS, the user information, and applications.

It establishes the data structure that will hold the signals, flags and semaphores that are used to communicate within and between the subsystems and applications of the computer.

The Operating System's tasks, in the most general sense, falls into six categories.

* Process Management
* Memory Management
* Device Management
* Storage Management
* Application Interface
* User Interface

## Process Management

The OS decides which task or process gets the processor (CPU), when and how much time it will take, allocation and de-allocation of processor time to the processes when required, keeps track of the processor and the status of the process by a program called the traffic controller.

### Process Management Activities

* Creating and deleting both user and system processes
* Suspending and resuming processes
* Providing mechanisms for process synchronization
* Providing mechanisms for process communication (IPC -- Inter-process communication)
* Providing mechanisms for deadlock handling

## Memory Management

OS manages main memory, which provides a fast storage that can be accessed directly by the CPU. A program that has to be executed, must be mapped first into the main memory.

OS also keeps track of the main memory -- which parts are used and which are unused.

Allocation and de-allocation of main memory blocks is also done by the OS. Allocation of the memory to processes when it requests it and de-allocation of the memory at the end of the process lifecycle.

OS decides which process will get the memory when and in what amount.

## Device Management

* OS manages drive communication via their respective drivers
* OS decides which process gets device access at what time and for what duration
* Using I/O controller, OS keeps track of all devices and their (de)allocation.

## File Management

* The OS keeps track of status, location and uses of resources. Allocation of resources when required and de-allocation of resources when their work is completed is also the OS' job.

### Security and Protection

Preventing unauthorized access to programs and data, a defence of the system against internal and external attacks. These attacks include Denial-of-Service (DoS), viruses, identity theft, or theft of service.

#### Protection

A mechanism for controlling access of processes and users to resources defined by the OS.

## Error detection

Applications which allow standard communication between user and software with the help of OS error detecting mechanism.

## User Interface

Two types of user interfaces exist:

* CLI - Command Line Interface
* GUI - Graphical User Interface

The OS provides a GUI for higher functions without writing any commands. This allows us to communicate with the computer with the help of buttons, and cursors.
