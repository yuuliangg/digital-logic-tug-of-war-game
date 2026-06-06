# Digital Logic Tug-of-War Game

## Overview
This project is a two-player Tug-of-War style game built using digital logic circuits. Players press buttons to move a shared counter up or down, and the game determines the winning side based on predefined counter thresholds.

The project demonstrates digital logic design, counter-based game mechanics, seven-segment display interfacing, comparator-style decision logic, and physical circuit board testing.

## Project Concept
The game starts from a middle value of **20**.

- Player 1 presses a button to increase the counter towards **30**.
- Player 2 presses a button to decrease the counter towards **10**.
- When the counter reaches the target threshold, the corresponding player scores.
- The design uses counter logic, display decoding, gate logic, and win-condition detection to create a simple competitive hardware game.

## Tools and Components
- Digital logic ICs
- Logic gates
- Counter ICs
- Seven-segment display drivers
- Push buttons
- Circuit board / breadboard testing
- TINA simulation / circuit design environment

## Key Technical Features
- Two-player button input system
- Counter-based game state
- Seven-segment display output
- Win-condition detection at upper and lower counter thresholds
- Logic-gate control for game flow
- Hardware prototype testing and troubleshooting

## Design Challenges
During implementation, several hardware and logic issues had to be addressed:

- Switch bounce causing multiple or missed counts per press
- Counter digit errors caused by incorrect carry/borrow handling
- Asynchronous LOAD / CLR controls causing unexpected resets or presets
- Win-condition logic triggering one count too late
- Unstable preset behaviour when loading the starting value
- Signal integrity differences between simulation and physical hardware

## What I Learned
This project helped strengthen my understanding of digital logic beyond theory. Building the game required translating game rules into hardware logic, testing behaviour on a physical circuit, and debugging issues that do not always appear in simulation, such as switch bounce, unstable inputs, and timing-related glitches.

## Repository Structure
```text
digital-logic-tug-of-war-game/
├── README.md
├── screenshots/
│   ├── 01-project-overview.png
│   ├── 02-game-mechanics.png
│   ├── 03-main-logic-circuit-schematic.png
│   ├── 04-counter-display-circuit-schematic.png
│   └── 05-testing-and-troubleshooting.png
├── docs/
│   ├── project_explanation.md
│   └── troubleshooting_notes.md
└── presentation/
    └── README.md
```

## Notes
The original editable schematic file is not available, so this repository documents the project using preserved schematic screenshots, presentation screenshots, project explanation, and troubleshooting notes.
