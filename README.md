# Minecraft Redstone Computer

![1](https://github.com/OliverW147/Minecraft-Redstone-Computer/blob/main/1.png?raw=true)

This project showcases a Minecraft-based computer I designed (mostly) and built mainly over y11 school holidays using Redstone logic gates, latches, and clocks. The computer uses basic components like Redstone Wire, Redstone Torches, Repeaters, and Comparators to form a fully functional system. The aim of this build was to create a simple computer within Minecraft, including elements like ROM, RAM, an ALU, a program counter, and a display system.

## Computer Overview

The computer features:

- **ROM (Instruction Memory)**: 64 registers with 33 bits each for storing instructions.
- **RAM**: 2 RAM modules, each containing 7 registers and capable of storing 8-bit values.
- **ALU (Arithmetic Logic Unit)**: Performs basic arithmetic and logical operations such as AND, OR, XOR, NOT, ADD, SUBTRACT, and conditional branching.
- **Magnitude Comparator**: Compares two 8-bit values for equality or magnitude.
- **Clock**: Operates at a 36-second clock cycle (0.027 Hz).
- **Program Counter**: Supports conditional and unconditional branching.
- **Display**: A 7-segment display used to visualise 4-bit digits after double dabble algorithm.
- **Fibonacci Sequence Example**: As a demonstration of the computer’s capabilities, the Fibonacci sequence was implemented with instructions to load values, perform operations, and store results in memory.

## Components Used

### Redstone Components:
- **Redstone Wire**: Used to transmit power signals, with repeaters required to boost the signal every 15 blocks.
- **Redstone Torches**: Act as power sources and can be used as inverters (NOT gates) in logic circuits.
- **Redstone Repeaters**: Used for signal boosting and adding delay, essential for timing and latches.
- **Redstone Comparators**: Compare and subtract signals, useful for creating magnitude comparators and conditional logic.

## Design Notes

While I designed an ALU and most of the components, I used three pre-existing designs to optimise space and improve performance. Specifically:

- **Program Counter**: I adapted a pre-existing design for the program counter, which was sourced from the internet. I modified the design to incorporate a clock and support for conditional branching.
- **Binary to BCD Converter**: A standard design was used for converting 8-bit values to Binary-Coded Decimal (BCD).
- **ALU**: Although I designed my own ALU, I opted for a more compact and efficient version created by **n00b_asaurus**. This design greatly reduced space usage and increased the clock speed of the computer.

## License

This project is licensed under the MIT License.
