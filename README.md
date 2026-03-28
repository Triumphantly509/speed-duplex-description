# Configuring switch interfaces, speed, duplex, description

## Objective
The objective of this lab is to practice configuring and verifying speed and duplex settings on a switch interface, simulate a duplex mismatch, observe its impact on network connectivity, and restore proper communication by correcting the interface configuration.

## Skills learned
- Switch interface configuration (speed and duplex)
- Network connectivity testing using ping
- Troubleshooting duplex mismatch issues
- Using Cisco IOS verification commands (show interfaces, show interfaces status)
- Understanding Ethernet communication behavior in different duplex modes
  
## Tools used
- Cisco Packet Tracer
- Cisco 2960 Switch
- PC Hosts
- Cisco IOS CLI

## Commands Practiced
- enable
- configure terminal
- interface FastEthernet0/1
- speed 100
- duplex half
- speed auto
- uplex auto
- no shutdown
- show interfaces FastEthernet0/1
- show interfaces stat
  
## Lab Topology
<img width="600" alt="image" src="https://github.com/user-attachments/assets/9ec3cb07-7942-4b82-a0e1-ac71e6471b0d" />


## Check speed and duplex on the switch
<img width="600" height="271" alt="image" src="https://github.com/user-attachments/assets/97178409-9434-44b0-bcdb-ebc98916b4fc" />

## Check the speed and duplex configuration on FastEthernet0/1
<img width="600" alt="image" src="https://github.com/user-attachments/assets/62726f21-287f-44b4-969f-a7f13fab6808" />

## Create a Duplex Mismatch

### Force HALF duplex on the switch
<img width="600" alt="image" src="https://github.com/user-attachments/assets/4681943c-7014-4b75-b73c-b6667987de72" />

### Verify
<img width="600" alt="image" src="https://github.com/user-attachments/assets/8ee2e7e2-b19f-4453-a1af-8c72d4869f48" />

### Force FULL duplex on PC0
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d887b750-d0d2-411f-9b67-42cbbc68cc5c" />

### Test with ping
<img width="600" alt="image" src="https://github.com/user-attachments/assets/03b8609c-d7d5-4512-8fe9-5e327b440757" />

A duplex mismatch occurs when two connected devices operate in different duplex modes (one full-duplex and the other half-duplex). This can lead to collisions, late collisions, and degraded network performance.

### Restore matching duplex settings.

### Option 1: Set both sides to auto negotiation.

### On the switch side
<img width="600" alt="image" src="https://github.com/user-attachments/assets/05fd71de-222c-44d6-bc43-d2820735ec29" />

### On PC0 side
<img width="600" alt="image" src="https://github.com/user-attachments/assets/617ea6d0-f21d-4cf1-a442-1bde935a561f" />

### Test with ping
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d658cea7-d166-4478-ae36-200b0318f82d" />


### Option 2: Set both sides manually to the same value.

### On the switch side
<img width="600" alt="image" src="https://github.com/user-attachments/assets/cfbc34b8-6c3f-43c6-90c0-a6f6d88f71b4" />

### On PC0 side
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f929d580-c761-414c-b65d-1cd4eb9e3fcd" />

### Test with ping
<img width="600" alt="image" src="https://github.com/user-attachments/assets/46e6a92c-1fc1-4dbd-a6e6-d696a102ebfd" />

### status with description
<img width="600"  alt="image" src="https://github.com/user-attachments/assets/f5286743-8059-4b99-8383-d2a16b0e4f99" />











