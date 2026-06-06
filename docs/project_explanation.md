# Project Explanation

## Objective
The objective of this project was to build a simple interactive game using digital logic circuits instead of software. The game had to be competitive, easy to understand, and able to demonstrate real hardware behaviour.

## Game Logic
The chosen concept was a two-player Tug-of-War game.

The counter starts at 20:
- Player 1 pushes the value upwards.
- Player 2 pushes the value downwards.
- Player 1 wins when the value reaches 30.
- Player 2 wins when the value reaches 10.

The system therefore needs to:
1. Accept button inputs from two players.
2. Update the counter correctly.
3. Display the value using seven-segment displays.
4. Detect the win condition.
5. Reset or prepare for the next round after a point is scored.

## Hardware Logic
The circuit uses a combination of:
- Counters for the current game value
- Seven-segment display driver ICs for visual output
- Logic gates for control conditions
- Button inputs for player actions
- Decode logic for threshold detection

## Implementation Focus
A major part of the project was not just building the intended circuit, but debugging real hardware behaviour. Physical buttons and digital ICs can behave differently from ideal simulation models, especially when there are floating inputs, long connections, timing issues, and switch bounce.

## Engineering Takeaway
This project gave practical experience in digital systems design, especially the difference between a circuit that works logically on paper and one that behaves reliably on physical hardware.
