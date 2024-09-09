# CS3100 Notes 09/09/2024

## System Calls
- Fork the way we create a new process
- To Create a process it must be created from another process
- Command: **man fork**

### What Happens When We Make A System Call
Cloud - User Application \
open() - System Call to Open A File \
User Calls Open on System Call interface Table \ 
Returns to the application then to the cloud

### strace
command to see the system calls from commands run in the konsole

### Types/Examples
- Process Control
  - Capabilities: Create, Terminate, Synchronize, Debug
  
- Calls
  - Capabilities: Fork, Exit, Wait
  
- File Management
  - Capabilities: Create/Delete file/folders, permission handling, Open Close
  - Calls: open, read, write, close, mkdir

- Device Management
  - Capabilities: Request/release device, read/write, attach/detach
  - Calls: read, write, ioctl

- Info Maintenance
  - Capabilities: Get/Sey date/time, get/set system data, get/set process/file/device info
  - calls: Getpid, alarm, sleep, getcwd

- communications
  - Capabilities: create/delete comm connections, send/rec info
  - Calls: pipe(), kill()

- Protections 
  - Capabilities: File Perms
  - Calls: chmod, chown, chroot

## Function Call Stack
Stacks and Heaps

1. User Program \
2. Register, Block in Memory, Parameters on a Stack \
3. Operating System

- \2. is used to pass the data back and forth

Registers
- fast
- small
- few of them

Block in Memory
- Slow
- Large
- Can Pass a Table
    - Overcomes "Few of them" Issue

Parameters on a Stack
- Slow


### test acronym
Symmetric High Speed Electric Transfer is not the answer
