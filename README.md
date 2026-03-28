# Configuring switch interfaces, speed, duplex, description

## Objective
The objective of this lab is to configure and manage switch interfaces on a Layer 2 switch. This includes enabling interfaces, configuring interface descriptions, manually setting interface speed and duplex mode, and verifying the configuration using Cisco IOS commands. These configurations help ensure proper link performance and provide clear documentation of switch ports.

## Skills learned
- Configuring switch interfaces

- Enabling switch ports using no shutdown

- Configuring interface descriptions for documentation

- Manually configuring speed and duplex settings

- Navigating the Cisco IOS CLI

- Verifying interface configurations

- Understanding how duplex mismatches affect network performance

- Performing basic interface management and troubleshooting
  
## Tools used

## Commands Practiced

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

### Option 2: Set both sides manually to the same value.









