# Day 7: Timing Analysis - Setup and Hold Constraints

## Concepts Mastered:
1. **Setup Time ($T_{su}$):** Minimum time data must be stable before the clock edge. Determines the Max Frequency ($F_{max}$).
2. **Hold Time ($T_h$):** Minimum time data must remain stable after the clock edge. Independent of clock frequency.
3. **Slack Calculation:** - **Setup Slack:** $T_{clk} - (T_{c2q} + T_{comb} + T_{su})$
   - **Hold Slack:** $(T_{c2q} + T_{comb}) - T_h$
4. **Metastability:** The "Illegal" state when timing is violated, resolved using multi-stage synchronizers.

## Takeaway:
Setup violations can be fixed by slowing down the clock ($F_{max}$), but Hold violations are independent of clock speed and must be fixed by adding physical delay (buffers) to the data path.
