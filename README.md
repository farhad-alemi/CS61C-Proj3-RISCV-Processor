# CS61CPU

Look, I made a CPU! Here's what I did:

- ALU: Implemented RISC-V instructions. In this part, digital logics was used to implement the instructions.

- RegFile: Implemented all the 32 registers in the ISA. It first feeds the input to the processor(s) keeping in mind only to turn on the procssors specified; i.e. without affecting the others.

- CPU: Assembled sub-components into a single processing unit. Immediate generator was implemented such that it extracts the immediate from various instruction forms appropriately.

- ImmGen: The immediate generator component uses a mux to specify which immediate generation process to follow based on the value from ImmSel.

- BranchComparator: Uses two comparators, unsigned and 2's complement, to compare and set the flags appropriately.

- Control Logic: Uses logic gates to identify various instructions and sets control flags appropriately.

- CSR: This module is added for testing purposes.

- The CPU has been pipelined and has two stages.