# Minecraft Redstone Computer

![1](https://github.com/OliverW147/Minecraft-Redstone-Computer/blob/main/1.png?raw=true)

This project showcases a Minecraft-based computer built mainly over y11 school holidays using Redstone logic gates, latches, and clocks. The computer operates with basic components like Redstone Wire, Redstone Torches, Repeaters, and Comparators to form a fully functional system. The aim of this build was to construct a simple computational system within Minecraft, including elements like ROM, RAM, an ALU, a program counter, and a display system.

## Computer Overview

The computer features:

- **ROM (Instruction Memory)**: 64 registers with 33 words each for storing instructions.
- **RAM**: 2 RAM modules, each containing 7 registers and capable of storing 8-bit values.
- **ALU (Arithmetic Logic Unit)**: Performs basic arithmetic and logical operations such as AND, OR, XOR, NOT, ADD, SUBTRACT, and conditional branching.
- **Magnitude Comparator**: Compares two 8-bit values for equality or magnitude.
- **Clock**: Operates at a 36-second clock cycle (0.027 Hz).
- **Program Counter**: Supports conditional and unconditional branching, allowing the program to jump to different instructions based on conditions.
- **Display**: A 7-segment display that converts 8-bit values to base 10 for visualization.

## Design Notes

While I designed an ALU and most of the components, I used three pre-existing designs to optimize space and improve performance. Specifically:

- **Program Counter**: I adapted a pre-existing design for the program counter, which was sourced from the internet. This design was modified to incorporate a clock and support for conditional branching.
  
- **BCD to Binary Converter**: A standard design was used for converting 8-bit values to Binary-Coded Decimal (BCD), which is essential for driving the 7-segment display.
  
- **ALU**: Although I initially designed my own ALU, I opted for a more compact and efficient version created by the user **n00b_asaurus**. This design greatly reduced space usage and increased the clock speed of the computer.

## Components Used

### Redstone Components:
- **Redstone Wire**: Used to transmit power signals, with repeaters required to boost the signal every 15 blocks.
- **Redstone Torches**: Act as power sources and can be used as inverters (NOT gates) in logic circuits.
- **Redstone Repeaters**: Used for signal boosting and adding delay, essential for timing and latches.
- **Redstone Comparators**: Compare and subtract signals, useful for creating magnitude comparators and conditional logic.

### Memory and Logic:
- **ROM (Instruction Memory)**: 64 registers, each storing a 33-bit instruction.
- **RAM**: Two 7-register memory modules capable of holding 8-bit values.
- **ALU**: Performs various arithmetic and logical operations.
- **Magnitude Comparator (MGC)**: Used for comparing values in memory.
  
### Display:
- **7-Segment Display**: Outputs values from RAM in base 10 format after conversion via a Binary-Coded Decimal (BCD) algorithm. The algorithm used is the Double Dabble method, and it ensures that values from the 8-bit register are displayed correctly.

## Features and Functionality

- **Clock**: The computer operates with a slow clock speed of 36 seconds per cycle, reflecting the limitations of Minecraft Redstone in terms of processing speed.
- **Branching**: Supports both conditional and unconditional jumps based on comparison results, allowing for simple control flow in programs.
- **Cache**: Stores the last operation result for easy retrieval, optimizing program execution.
- **Operations**: The ALU supports several basic operations, including arithmetic (ADD, SUBTRACT) and logical operations (AND, OR, XOR, NOT).
- **Fibonacci Sequence Example**: As a demonstration of the computer’s capabilities, the Fibonacci sequence was implemented with instructions to load values, perform operations, and store results in memory.

## Performance Considerations

- **Clock Speed**: Due to the large number of Redstone components, the clock cycle is relatively slow, and performance is limited to basic operations.
- **Space Optimization**: The use of the ALU design from **n00b_asaurus** and the program counter modification allowed for significant space-saving, making the build more compact and faster.

## Acknowledgements

- **n00b_asaurus**: For the ALU design, which greatly reduced space and increased clock speed.
- **Program Counter and BCD to Binary Converter**: While I contributed to the build, the designs for the program counter and BCD conversion were sourced from the internet to ensure efficiency and simplicity.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
