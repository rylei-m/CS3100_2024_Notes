# Operating Systems 08/30/2024

## Storage Structure

### Memory
The CPU can Access Directly
- Main Memory
- Registers
- Memory Cache
- RAM - Random Access Memory
- Volatile

### Secondary Storage
- Mechanical
- HHD

#### Electrical
- SSD
- Non-Volatile Memory
- Fast
- Predictable

## I/O Structure

### Interrupts
After Every Instruction the Computer Checks for an Interrupt
- An Emergency - Something like a Keyboard Interrupt

#### Implementation
ISR - Interrupt Service Routine
- A Set of Instructions \
IV - Interrupt Vector
- Array of Addressed for the ISR \
Terminology
- Raises an Interrupt
- CPU Catches/Dispatches an Interrupt Handler

## OS Operations
1) Bootstrap
   - Boot Loader
   - Initializes Hardware
   - Load OS