# OS Architeture
There's the *Level Machine*:
![Level Machine](https://raw.githubusercontent.com/saukennn/sauk-hat/main/assets/levelMachine.png)

Levels 0, 1, 2, 3, 4: Low level, level 0 is the real machine.
Levels 5 and 6: High level.

The OS is formed with several routines, that together are called system core, or kernel.
## Kernel roles:
1. `Scheduling and communication between processes` - The kernel ensures that multiple processes can run simultaneously by using scheduling algorithms like Round-Robin or Priority Scheduling. It also allows inter-process communication (IPC) through message passing and shared memory
2. `Interrupt handling(system calls)` - When a user program tries to read a file, it triggers a system call, which the kernel handles by switching to kernel mode and accessing the requested file on disk. Similarly, when a hardware interrupt occurs (e.g., a keyboard press), the kernel processes the event and sends it to the appropriate driver.
3. `CPU management` - The kernel's CPU scheduler decides which process gets CPU time next. For example, in a multitasking system, if a process is executing an infinite loop, the kernel preempts it and assigns the CPU to another process to maintain system responsiveness.
4. `Memory management` - The kernel manages RAM allocation using techniques like paging and segmentation. If a program requests more memory than available, the kernel might use virtual memory, swapping less-used memory pages to disk
5. `Archive systems management` - When a user saves a document, the kernel interacts with the file system (e.g., NTFS, ext4) to store the data efficiently on disk. It also manages file permissions, ensuring that users cannot access restricted files.
6. `Input/Output devices management` - When a user prints a document, the kernel communicates with the printer driver to send the print job. It also manages other I/O devices, like USB drives and network interfaces, ensuring smooth data transfer between hardware and software.

### System access mode
Used to protect the system core (kernel), there're 2 types:
- User mode
- Kernel mode

### System activation
The OS is in the secondary memory (SSD-Solid State Driver or in HD-Hard disk). When you turn on the computer the OS needs to be loaded for the main memory (RAM-Random Access Memory), who is responsible for this is ROM-Read Only Memory, this component has a recorded process called system activation using the boot loader.
**Boot Loader, what is this?:**
It's a program that initialize the OS, is started when the computer is turned on or restarted. Bootloader functions:
- Initialize hardware.
- Load operating system.
-  Manage boot.
-  Manage recovery in case of errors.
-  Allow installation of alternative versions of the operating system.

So the proccess to activate the system in summary is: ROM ---> Secondary Memory ---> Main Memory
![ROM image](https://raw.githubusercontent.com/saukennn/sauk-hat/main/assets/readOnlyMemory.png)

**OS Languages**
The biggest part of OS's are builded in C or C++, previously it was in assembly, but they became completely dependent on the hardware. Designers still using assembly for drivers and treatment routines.

## Architecture Types
### Monolithic architetcture
Used in the first OS's tais such as CP/M, MS-DOS and initial Linux versions.
