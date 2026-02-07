# MAC Flooding – Technical Explanation

## How a Switch Works
A switch uses a CAM (Content Addressable Memory) table to map MAC addresses
to physical ports.

## How the Attack Works
The attacker sends thousands of Ethernet frames with random source MAC addresses.
The switch stores them until the CAM table becomes full.

## Result
Once the CAM table is full:
- The switch cannot learn new MAC addresses
- Frames are broadcast to all ports
- Confidential traffic can be intercepted
