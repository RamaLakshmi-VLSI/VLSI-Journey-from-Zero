# Day 6: FSM Application & Design Practice

## Design Problems Solved:
1. **Vending Machine Controller (Event-Driven):**
   - Designed a system to detect a 15-rupee total using 5 and 10 rupee inputs.
   - Performed manual Logic Synthesis by deriving the **Next State Equations** ($D_1, D_0$) and **Output Logic** ($Z$).
   - Analyzed state transitions for a Moore machine implementation.

2. **Traffic Light Controller (Time-Driven):**
   - Designed a 3-state (Green, Yellow, Red) controller based on a timer signal.
   - Evaluated the benefits of **One-Hot Encoding** for driving physical peripherals directly.

## Key Takeaway:
In VLSI, an FSM is not just a drawing; it is a balance of **Power, Performance, and Area (PPA)**. 
- Using **Binary Encoding** for the Vending Machine saved **Area** (fewer Flip-Flops). 
- Using **One-Hot Encoding** for the Traffic Light increased **Performance** (simple logic, higher speed) and simplified the output hardware.
A good designer doesn't just make the circuit work; they choose the architecture that fits the specific constraints of the system.
