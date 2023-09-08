# tec-Memory-Bank-Switching


When designing a memory bank controller for a Z80 Single Board Computer (SBC), you'll typically need an IC or circuit that can handle memory bank switching to expand the addressable memory space. A common choice is to use a memory mapper or memory management unit (MMU) that allows you to switch between different memory banks to access additional memory. Here are some options and considerations:

1. **74LS612/74LS614 Memory Mapper**:
   - These are simple memory mapper ICs designed specifically for Z80 systems. They provide memory banking capabilities, allowing you to access multiple ROM or RAM banks.
   - The 74LS612 supports up to 4 banks, while the 74LS614 supports up to 8 banks.
   - They are relatively easy to interface with the Z80 and are widely used in retro computing projects.

2. **Custom Logic with GAL or CPLD**:
   - If you have specific requirements and need more flexibility, you can design custom memory bank control logic using a Generic Array Logic (GAL) or Complex Programmable Logic Device (CPLD).
   - This approach allows you to implement custom bank switching logic tailored to your SBC's memory layout.

3. **FPGA**:
   - For even greater flexibility and functionality, consider using an FPGA (Field-Programmable Gate Array) to implement memory bank control.
   - FPGAs offer a high level of customization and can be configured to support various memory layouts and bank switching schemes.

4. **EPROM or Flash Memory with Address Decoding**:
   - Another approach is to use EPROM or flash memory chips with address decoding logic to create a bank switching mechanism.
   - By manipulating the chip enable (CE) or output enable (OE) pins of these memory chips, you can select different memory banks.

5. **Memory Controller ICs**:
   - Some memory controller ICs, such as the Intel 8284A Clock Generator and Driver for 8086/8088 Systems, can be adapted for memory bank switching purposes.
   - While not designed specifically for Z80 systems, they can still be used to generate control signals for memory bank switching.

6. **Commercial Memory Mapper ICs**:
   - In some cases, you may find commercial memory mapper ICs designed for retro computing or embedded systems. These ICs can simplify memory expansion in your SBC.

Remember that your choice of memory bank controller will depend on the specific requirements of your Z80 SBC project, including the number of memory banks needed, the memory size per bank, and the overall system architecture. Additionally, ensure that the selected memory bank controller is compatible with the Z80 processor and can be integrated into your SBC's design.

## 74LS612 

## Ref
- https://en.wikipedia.org/wiki/Bank_switching
- https://b13rg.github.io/Gameboy-MBC-Analysis/
- 
