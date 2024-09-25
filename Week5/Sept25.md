
Indirect Communication
- Mailboxes
- Sharing
- Uni or Bi-Directional

Synchronization
- Blocking
  - Synchronous - Cooperation between sender and receiver
  - Blocking Send - Cannot progress until counterpart is received
    - Singing Telegram
  - Blocking Receive - Cannot progress until counterpart is sent
    - Bus Stop
- Non-Blocking
  - Asynchronous - Sender and Receiver Don't Require Coordination
    - Non-Blocking Send - Ready or Not it will be Waiting for you
      - Regular Post Office 
    - Non-Blocking Receive - The Receiver Checks if Something is there and Takes it if Something is there, If not they will Just move on
      - Blue Mail Drop Off
- Any Mix is Possible
  - Send and Receive Blocking is called Rendezvous

Buffering
- Zero Capacity - Nowhere to Store Anything
  - Must Rendezvous
- Bounded Capacity
  - Must Blocking Send When Full
- Unbounded Capacity
  - Sender Never Blocks
  - Networking

Pipes
- Java Limitations
- Unix/C++
  - Two Types
    - Ordinary
      - Create a Pipe
      - Fork a Process
      - Uni-Directional
      - Bi- Directional
        - Make Two Pipes
    - Named Pipes
      - Created by One Process, Accessed by Many
      - Can be Bi-Directional
      - Looks Like a File

Sockets
- Network Programming
- IP - Computer Identifier
- Port - Mailbox for a Process

Remote Procedure Call/Remote Method Invocation
- Client Needs Computation
- Sends Parameters to Server
- Server Computes



Irrelevant Info
- Types of IPC
  - POSIX API - Shared Memory
  - Mach Message Passing
  - Windows Local Procedure Calls