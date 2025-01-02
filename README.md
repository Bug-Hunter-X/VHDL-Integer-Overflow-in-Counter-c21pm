# VHDL Integer Overflow Bug
This repository demonstrates a common error in VHDL: integer overflow in a counter. The `counter_bug.vhdl` file contains a counter that increments until it overflows. The `counter_solution.vhdl` file shows how to correct this issue using a modulo operator to wrap around the counter when it reaches the maximum value.

## Bug Description
The provided VHDL code implements a simple counter. However, it does not handle the case where the counter reaches its maximum value (15 in this example). When the counter attempts to increment past 15, an overflow occurs, leading to unpredictable behavior in simulation or synthesis. 

## Solution
The solution involves using the modulo operator to ensure the counter wraps around to 0 once it reaches 15. This prevents the overflow and guarantees correct counter behavior.

## How to reproduce
Simulate `counter_bug.vhdl` to observe the overflow error.  Compare the results to the simulation of `counter_solution.vhdl` to see the correct functionality.