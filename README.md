# Controller-Area-Network (CAN) Protocol Repository

This repository contains multiple case studies demonstrating the use of the Controller Area Network (CAN) protocol in embedded systems and simulations. The case studies explore CAN communication in both hardware and simulation environments, with different use cases involving data transmission and reception between ECUs.

## Case Studies

### 1. CAN-CASE-Study-1: STM32 CAN_MODE_LOOPBACK (Simulated in Keil MicroVision)
This project demonstrates a simple CAN communication setup in **CAN_MODE_LOOPBACK** using an STM32 microcontroller, simulated in **Keil MicroVision**. The system sends and receives the same data over the CAN bus to verify correct transmission and reception.

- **Purpose**: 
  The CAN loopback mode is useful for verifying that CAN communication is functioning correctly without needing a second device or node on the CAN bus.

### 2. CAN-CASE-Study-2: ECU-to-ECU Communication (Acceleration and Speed Control)
In this project, two ECUs communicate over the CAN bus.

- **ECU1**: Sends an acceleration indicator, which is either `0` (no acceleration) or `1` (acceleration).
  
- **ECU2**: Receives the acceleration indicator and adjusts the vehicle speed:
  - If the acceleration indicator is `1`, the speed is incremented.
  - If the acceleration indicator is `0`, the speed is decremented.

- **Purpose**: 
  This case study simulates a real-world scenario of communication between different control units in a vehicle, where one ECU monitors acceleration and another controls speed accordingly.

### 3. CAN-CASE-Study-4: CANoe Simulation with GUI and Database
This case study is similar to **CAN-CASE-Study-2** but implemented using **CANoe simulation**, with additional features such as a graphical user interface (GUI) and a database for logging.

- **Components**:
  - A **switch** in the GUI controls the acceleration indicator.
  - An **analog indicator** in the GUI represents the vehicle speed.
  
- **Purpose**: 
  This simulation demonstrates the use of CANoe for visualizing and testing CAN communication in a more user-friendly and flexible environment, allowing for easier manipulation of input (acceleration) and observation of output (speed).

## Contact
For any inquiries or issues, feel free to contact the repository owner at [abdo01445@gmail.com](mailto:abdo01445@gmail.com).