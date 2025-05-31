## Modbus Packet Analysis Lab

**Tools used**: OpenPLC, Wireshark  
**Objective**: Capture and analyze Modbus TCP traffic.

### Steps:
1. Ran OpenPLC server and HMI client on localhost
2. Captured traffic using Wireshark with filter: `tcp.port == 502`
3. Observed Modbus function codes (0x03 Read Holding Registers)
4. Identified a simulated replay attack by repeating packet with function 0x06

### Screenshot:
![Modbus Traffic Screenshot](../assets/diagrams/modbus-traffic.png)
