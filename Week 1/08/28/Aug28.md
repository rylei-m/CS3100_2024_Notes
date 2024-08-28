# Operating Systems 08/28/2024
Present interface to user
manage computer hardware
resource allocator


## Two Views
### User Views
- ease of use
- good performance
  - fast
  - long battery life
- Some systems have little to no user view, such as embedded computers
  - Cars, Home Devices, etc
  - Light, Keypad

### System Views
- Resource Allocator
- Manage Conflicting Requests
- Efficient hardware use

## Kernel
The Parts that always have to be running
- The file system \
Embedded Systems may not have a file system

## Computer Organization
### Processing Units
Each Processor in a Computer has its own Processor and Cache, and they are Connected by the Bus \
Advantages to Having 2 CPUs
- Parallelism - The ability to do two things at the same time. Ex: your roommate cleans the dishes, you vacuum
- Through Put - The actual amount of tasks being performed is a time measurement
- Coordination - CPU manage how the bus is organized.
#### Asymmetric Multi-processing
The processors activities are not equal \
One CPU is the "boss."
- Manages who does what
- Manages what the other processor does \
Issue: The CPU can get **too** busy and not effectively control tge other CPU
#### Symmetric Multiprocessing
Either processor can do anything
- Equal Access to Memory
- Have to Coordinate Tasks Through Extra Overhead
  - Overhead: The Extra Costs that you Incur in Order for you to Operate

## Single Processor with 2 CPU Cores
Separate brains that combine to share cache before reaching the main memory
- Faster than accessing main memory
- Requires More Coordination

## Clustered Systems
### Super Computers/High Performance \
A group of systems tied together to performance a single task

## Cache
Temporary Storage Space
