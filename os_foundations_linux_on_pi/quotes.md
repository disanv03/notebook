# Operating Systems Foundations with Linux on the Raspberry Pi

## A Memory-centric system model

The purpose is to help you understand that in a processor-based system, all actions fundamentally reduce to operations on addresses.

This is a very important point: _every observable action in a processor-based system is the result of writing to or reading from an address location._


Definition of processor from [foldoc]:
> The part of a computer which controls all the other parts.

#### What does the processor do ?

The processor is a machine to modify the system state.
- A key feature of a processor is the ability to run arbitrary programs
- A program consists of a series of instructions
- An instruction determines how the processor interacts with the system through the address space: it can read values at given address, compute new values and address, and write values to given addresses.


#### Procesor internal state: registers

Although in principle, a processor could directly manipulate the system state, this is not practical because DRAM memory access is quite slow. Therefore, in practice, processors have a dedicated internal state known as the register file, an array of words called registers which you can consider as a small but  very fast memory.
