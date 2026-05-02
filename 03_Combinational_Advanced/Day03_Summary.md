# Day 3: Advanced Combinational Blocks

## Concepts Covered:
* **MUX Logic:** Mastered the "Block Observation Method" to implement any logic function using Multiplexers.
* **Arithmetic Units:** Derived Full Adder (Sum and Carry) and Full Subtractor logic.
* **Ripple Carry Adder (RCA):** Analyzed the architecture and the trade-off between bit-width and propagation delay ($T_{pd}$). 
* **Decoders:** Learned minterm generation and implementation. 
    * *Active High Decoder:* Use OR gates to combine minterms.
    * *Active Low Decoder:* Use NAND gates to combine minterms.
* **Priority Encoders:** Solved the ambiguity of multiple inputs using "Don't Cares" (X) and the Valid Bit (V).

## Practice Problem & Derivations:

### 1. Full Adder Carry-out (4:1 MUX)
* **Task:** Implement $C_{out}$ with $A, B$ as Select Lines.
* **Inputs:** $I_0 = 0$, $I_1 = C_{in}$, $I_2 = C_{in}$, $I_3 = 1$.

### 2. Logic Implementation via Decoder
* **Task:** Implement $F(A, B) = \sum m(1, 2)$ using a 2:4 Active High Decoder.
* **Solution:** Connect outputs $Y_1$ and $Y_2$ to a 2-input **OR gate**.

### 3. Priority Encoder Edge Case
* **Question:** In a 4:2 Priority Encoder, if $D_3 D_2 D_1 D_0 = 0000$, what are the values of $Y_1 Y_0$ and $V$?
* **Answer:** $Y_1 Y_0 = XX$ (Don't Care) and **$V = 0$** (Invalid). 
* **Reasoning:** The $V$ bit is necessary to distinguish this "no input" state from the "Input 0" state ($0001 \rightarrow Y=00, V=1$).
