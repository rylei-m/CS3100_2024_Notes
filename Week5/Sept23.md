# Notes 09/23/2024

Android
- Foreground
- Visible
- Service
- Background
- Empty

Interprocess Communication
- IPC 
  - Types:
    - Independent
    - Cooperating
  - Reasons
    - Relies or is Relied On by Other Processes
    - Important for Computer Speed-Up
    - Modularity
  - Methods
    - Shared Memory
      - Producer - Consumer Model
      - Model 
        - Shared Buffer
        - No Direct Communication
      - Buffer
        - Constraints
          - Unbounded
            - Producer - No Waiting
            - Consumer - Wait if Empty
          - Bounded
            - Producer - Wait if Full
            - Consumer - Wait if Empty
    - Message Passing
      - Operations
        - Send
        - Receive
      - Model
        - Generate Message in Process A
        - Copy Message to System Call or to Process B
        - Direct or Indirect
      - Issues
        - How is the Link Established
        - How Many Links per Process
        - Message Size
        - Uni or Bi-Directional
        - Buffered or Non-Buffered
        - Blocking or Non-Blocking
      - Direct or Indirect Communication
        - Direct
          - Processes Must Know About Each Other
          - Properties
            - One Link
            - Automatically Established
            - One Pair of Processes
            - Normally Bi-Directional
          - Issue
            - Identifying processes
        - Indirect
          - "Mailboxes"
            - Unique Identifier
            - Processes Known About Mailboxes, Not Other Processes