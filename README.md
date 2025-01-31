# VHDL Counter Off-by-One Error
This repository demonstrates a common off-by-one error in VHDL counters and provides a solution.

## Bug Description
The provided VHDL code implements a counter that is supposed to count from 0 to 15. However, due to an error in the code, the counter does not reach the value 15 before resetting to 0. This leads to an incorrect counting behavior. 

## Solution
The solution involves correcting the condition in the 'if' statement within the process. The original condition `if count = 15 then` should be changed to `if count = 14 then` to properly reset the counter after it reaches its maximum value (15).