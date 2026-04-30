# Digital Password Checker (FSM Based)

## Overview
This project is a binary password verification system designed using concepts from Digital Logic Design. It validates a predefined binary password using sequential logic and state transitions.

The correct password is:
**1001**

The system is implemented using D Flip-Flops and follows a Finite State Machine (FSM) design approach.

---

## Features
- Binary password authentication using sequential input
- FSM-based design using D Flip-Flops
- Hardware implementation using breadboard
- Simulation using Logisim
- Output indicators using LEDs:
  - Blue LED: Correct password
  - Red LED: Incorrect attempt
  - Yellow LED: System locked after 3 consecutive wrong attempts
- Reset functionality to restore initial state

---

## System Description

### Correct Password Operation
The system checks the input sequence bit by bit. If the sequence matches 1001 exactly, the system transitions to a success state and activates the blue LED.

### Incorrect Password Operation
If the input sequence does not match the correct password, the system registers a wrong attempt and activates the red LED.

### Locking Mechanism
After three consecutive incorrect attempts, the system enters a locked state (state 11). In this state:
- The system stops processing inputs
- The yellow LED is activated
- The system remains locked until reset

### Reset Function
The reset button returns the system to its initial state (state 00) and clears all stored states and counters.

---

## Design Approach
The system is designed using:
- Sequential logic circuits
- D Flip-Flops
- Finite State Machine (FSM) principles

Each state transition depends on the current state and input bit, ensuring structured password validation.

---

## Implementation

### Hardware Implementation
The circuit is physically implemented using a breadboard with logic gates and D Flip-Flops.

Location: `implementation/`

---

### Simulation
The same design is implemented and verified using Logisim.

Location: `simulation/`

---

## Design Documentation

The following design elements are included:

- Truth Table: `design/truth_table.png`
- State Table: `design/state_table.png`
- State Diagram: `design/state_diagram.png`

---

## Project Structure

digital-password-checker/
│
├── README.md
├── implementation/
├── simulation/
├── design/
├── report/
└── media/

---

## Learning Outcomes
- Understanding of sequential logic design
- Implementation of FSM using D Flip-Flops
- Practical hardware circuit design
- Simulation and verification using Logisim
- Integration of theoretical and practical digital systems

---

## Future Improvements
- Keypad-based input system instead of binary switches
- Display output using 7-segment or LCD module
- Enhanced security with longer or dynamic passwords
- Automatic timeout-based lock system

---

## Author
Syed Tahsin Reza
