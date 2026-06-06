# Troubleshooting Notes

## Issue 1: Switch Bounce
Button presses sometimes caused multiple counts or missed counts. This was caused by mechanical switch bounce and wide button signal levels.

## Issue 2: Incorrect Digit Transition
The tens digit was affected by button input instead of being driven cleanly by carry/borrow logic from the units digit. This caused jumps such as 20 to 11.

## Issue 3: Asynchronous Control Glitches
LOAD, CLR, and win-decode signals sometimes caused unexpected presets or resets because they were not fully synchronised with the intended clock behaviour.

## Issue 4: Win Detection Timing
The win condition was sometimes detected after the clock edge, allowing the counter to move one extra count past the intended 10 or 30 threshold.

## Issue 5: Unstable Starting Value
The preset to 20 was unreliable when LOAD timing or preset lines were unstable.

## Issue 6: Simulation vs Hardware Differences
The circuit behaved differently in simulation and hardware due to threshold differences, floating inputs, wiring length, and signal integrity issues.
