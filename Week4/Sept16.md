# CS3100 Notes 09/16/2024

## TODO
- Assn3 - Due October 4th

## System Boot-Up

## BIOS: Basic Input Output System
- Order to Look at Devices
- Non-Volatile Read Only Memory
  - The Starting Point for Booting
  - Start up HD
  - Points to MBR

### Master Boot Record: What is On The HardDrive
- Located on HD
- Knows HD Formatting
- Pulls the OS into Memory

### Limitations
- Runs in 16-bit mode
  - You can only have so much memory
  - Standard Computers have 64
- Text based Interface
- Max HD of 2.1TB
- Only Init One HW Device at a Time
  - Slow
- Security Issues
  - RootKit Virus
  
## UEFI - Unified Extensible Firmware Interface
- 32 or 64 bit mode
- GUI Interface
- Mouse
- Init Many Hardware Devices
- Networking
  - Remote Management
- OS Validity Check
- Mini OS
- NO MBR (Master Boot Record)
  - GUID Partition Table
    - Globally Unique ID
    - The Unique Number of Everyone's Computer
    - Can Recover From Corruption

## Processes
- Program vs Process (executing)
  - A Program is on your hard drive but is just sitting there
  - A program loaded into memory is a process
- A Program 
  - is just a list of Instructions
- A Process
  - (max) Stack -> <- heap, data, text (0)
      - The Stack and Heap can change sides
      - Process Stacks - Only Used for Functions
      - Never Overlap Between Stack and Heap
      - Text - The Actual Instructions in 1s and 0s

## User Stack vs Kernel Stack
- User Processes are also created in the kernel
- Good for memory addressing
- Users cannot write directly on Kernel Stack

## Process States
- The Purpose of a process at an exact moment
- 13 Total States (Mostly Waiting)
- 5 Key States:
  - New
    - Created by a System Call
    - Immediately Goes to Ready State
  - Ready
    - It can be put on the CPU at Any Time
    - Scheduler moves process to running state
  - Waiting
    - If a process is running and needs data from hard drive but that data is not ready the state will go to waiting (I/O)
    - When I/O finished sends Interrupt to CPU returns state to ready
  - Running
    - Runs Until Timer Interrupt
    - then back to ready state
  - Terminated

## PCB - Process Control Blocks
- The View of The Process for the Operating System
- Data Structure the OS Uses to Manage a Process
