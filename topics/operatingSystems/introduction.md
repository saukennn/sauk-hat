# Introduction for Operating Systems

**1. System Programs**  
Softwares able to manage and control computer hardware, creating a base for other programs execution. Examples:
   - Operating systems (Windows, Linux, macOS)
   - Device drivers (printer controller, graphic card)
   - System utilities (antivirus, archive manager, backup tools)

**2. Application Programs**  
These are programs developed to meet specific user needs. Examples:
   - Productivity software (Microsoft Office, Google Docs)
   - Internet browsers (Google Chrome, Mozilla Firefox)
   - Games (Valorant, LoL, Dota, GTA)
   - Video and image editors (Adobe Photoshop, Premiere Pro, Sony Vegas)

**3. Computer Programs**  
Tools used to develop other software and make advanced calculations. Examples:
   - Compilers and interpreters (GCC, Python)
   - Integrated development environments (IDEs) (Visual Studio Code, IntelliJ IDEA)
   - Modeling and simulation software (MATLAB, AutoCAD)

## Operation of OS

**Processes (or Tasks)**  
- Basically, it is a running program.
- One process competes for CPU resources and interacts with other processes.
- They have three statuses: execution/running, blocked/waiting, or active/ready.
- The OS manages the processes with System Calls.

### What is System Calls?
System Calls are programming interfaces that allow running programs to request services from the kernel. SysCalls give us a high level of abstraction to access system resources. This allows programs to be developed independently of the hardware and OS they are running on.

Examples:
1. `open()` - Used to open a system file.
2. `read()` - Used to read data from a file.
3. `write()` - Used to write data to a file.
4. `close()` - Used to close a file.
5. `fork()` - Used to create a new process.
6. `exec()` - Used to replace the code of one process with another.
7. `exit()` - Used to terminate a process.

##Change of process state
<p align="center">
  <img src="assets/processesState.png">
</p>


