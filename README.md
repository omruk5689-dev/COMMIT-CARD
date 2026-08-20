Commit Card
<img width="2160" height="1236" alt="3D_PCB1_2026-08-21 (2)" src="https://github.com/user-attachments/assets/edfa5d05-d588-4f61-96af-b48aa95a3174" />

Commit Card is a compact, custom-designed NFC hardware project built around a microcontroller and an NFC tag IC. The idea is to create a programmable PCB in a card-like form factor that can communicate with NFC-enabled smartphones and readers.

 Features

- Custom-designed compact PCB
- On-board microcontroller
- Integrated NFC functionality
- NT3H2110 NFC tag interface
- SMD component design
- Designed for a compact card form factor
- Programmable hardware
- Open-source hardware project
- Designed from schematic to PCB

🔧 Hardware

The current design uses a combination of an MCU, NFC IC, resistors, capacitors, and supporting components.

Main Components

- MCU — Main processing and control unit of the Commit Card.
- NT3H2110W0FHAH — NFC tag IC used to provide NFC communication and memory functionality.
- 47 Ω resistors — Used within the signal/interface circuitry where required.
- 220 nF capacitors — Used for local decoupling and filtering around the ICs.
- U1 — Primary IC designation on the schematic/PCB.
- Additional passive components — Supporting resistors, capacitors, connections, and protection components required by the circuit.

«Component values and exact part numbers may change during PCB revisions and testing.»

 NFC System

The NT3H2110 is the main NFC component of the Commit Card.

It allows the PCB to interact with NFC-enabled devices such as smartphones and NFC readers.

The NFC section is integrated directly onto the PCB rather than using a separate NFC development module.

The intended communication flow is:

        ┌────────────────────┐
        │   Microcontroller  │
        │        MCU         │
        └─────────┬──────────┘
                  │
                  │ Digital Interface
                  │
        ┌─────────▼──────────┐
        │     NT3H2110       │
        │      NFC IC        │
        └─────────┬──────────┘
                  │
                  │ NFC
                  ▼
              Smartphone

 MCU

The microcontroller acts as the main controller of the Commit Card.

It is responsible for handling the logic of the board and communicating with the NFC IC.

The MCU can be used for:

- Processing card functions
- Communicating with the NFC IC
- Managing stored or exchanged data
- Running custom firmware
- Controlling future hardware features
- Providing a foundation for future revisions of the project

 Capacitors & Filtering

The PCB includes 220 nF capacitors for local power decoupling and filtering.

These capacitors help stabilize the supply around the ICs by reducing high-frequency noise and providing local transient current.

Proper placement close to the relevant IC power pins is important for reliable operation.

🔩 Resistors

The design includes 47 Ω resistors in the appropriate signal paths.

These can be used for signal conditioning, damping, or interface requirements depending on their exact location in the final schematic.

The final resistor values and placement will be verified during PCB testing.

 PCB Design

Commit Card is designed as a custom PCB rather than being assembled from development boards or breakout modules.

The PCB focuses on:

- Compact component placement
- Short signal paths
- Proper power distribution
- NFC antenna integration
- SMD assembly
- Card-style dimensions
- Clean and manufacturable routing

The PCB will go through schematic verification, layout checks, prototype manufacturing, assembly, and testing.

 Firmware

The firmware will control the MCU and provide the logic required for the card.

Planned firmware functionality includes:

- MCU initialization
- NFC communication
- Data handling
- Custom card functions
- Hardware testing
- Future expansion features


Commit Card is being developed as an open-source hardware project.

The design is intended to be publicly documented so others can study, modify, improve, and build upon the hardware.
