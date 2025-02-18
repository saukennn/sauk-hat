#Introduction for Operating Systems
    **1.System Programs**
    Softwares able to manage and control computer hardware, creating an base for other programs execution. Examples:
        - Operating systems (Windows, Linux, macOS)
        - Device drivers (printer controler, graphic card)
        - System utilities (antivirus, archive manager, backup tools)
    **2.Application Programs**
    These are programs delevoped to meet specific user needs. Examples:
        - Produtivity softwares (Microsoft Office, Google Docs)
        - Internet browsers (Google Chrome, Mozilla Firefox)
        - Games (Valorant, Lol, Dota, GTA)
        - Videa and image editors (Adobe Photoshop, Premiere Pro, Sony Vegas)
    **3.Computer Programs**
    Tools used to develop other softwares and make advanced calculations: Examples:
        - Compilers and interpreters (GCC, Python)
        - Integrated development environments (IDEs) (Visual Studio Code, IntelliJ IDEA)
        - Modeling and simulation softwares (MATLAB, AutoCAD)
##Operation of OS
    **Processes(or Tasks)**
        - Basically it is a running program
        - One process compete for CPU resources and interact with other processes
        - They have three status: execution/running, blocked/waiting or active/ready
        - OS manage the processes with System Calls.
            *What is System Calls?*
            + System Calls are programming interfaces that allow running programs to request services from kernel, SysCalls gave us an high abstration level to acess system resources, this resource make programs being developed independently which hardware and OS they running. Examples:
                1. open(): used to open an system archive
                2. read(): used to read data from archive
                3. write(): used to write data in an archive
                4. close(): used to close an archive
                5. fork(): used to create a new process
                6. exec(): used to replace the code of one process for other
                7. exit(): used to finish an process exec
