# What is booting process

Booting is the process that is used to load the operating system in memory. Data and programs remain stored on disk as permanent storage. But, because of slow access speed of physical disks, CPU interacts with main memory (temporary memory/RAM) to perform a task. Any program that needs to run must be loaded from disk into memory before it can be executed by the processor.

OS is the first system program to get executed and remains in the memory till the system execution. Before actual loading of the OS, BIOS routines play an important role. These routines perform a series of checks for reliability and availability of hardware attached. System BIOS is hardwired code on the motherboard.

The very first step of this is POST - Power On Self Test. It checks the validity of all hardware attached with the computer like mouse, keyboard, monitor, hard disk et cetera.

This is followed by another round of checks, this time on the memory area and non-peripheral devices.

Then, the bootstrap loader program is made available in the first physical sector of bootable disk by the Master Boot Record, also known as MBR.

The purpose of MBR is to find out the primary partition to load the boostrap loader into, for further processing.

## MS-DOS booting process

The booting sequence for the MSDOS operating system looks like the following flowchart.

```plaintext
BIOS Routines -> H/W Validity Check (Keyboard, Mouse, Monitor) -> Memory Check -> Non-standard Peripheral Check -> Master Boot Record (To check the partition in case of Disk) -> Loading of bootstrap loader -> IO.SYS (Disk BIOS, SYSINIT) -> MSDOS.SYS -> COMMAND.COM -> OS loaded in memory
```

MS-DOS OS has three core parts - `IO.SYS`, `MSDOS.SYS`, and `COMMAND.COM`.

### `IO.SYS`

`IO.SYS` contains the device drivers for various devices attached to the computer such as keyboard, mouse, et cetera.

### `MSDOS.SYS`

`MSDOS.SYS` is the interface between the user and the underlying hardware. All the major resource management roles performed by the OS are the part of this interface, like process management, file management, memory management et cetera.

### `COMMAND.COM`

`COMMAND.COM` is the command-line interface of MS-DOS. It is often referred to as 'shell'. It makes execution of all commands possible by the user.
