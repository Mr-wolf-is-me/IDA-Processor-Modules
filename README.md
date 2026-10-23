# IDA Processor Modules for Uncommon Architectures

A collection of processor modules extending **IDA Pro** with support for uncommon and specialized CPU, DSP, and GPU architectures.

These projects grew out of my interest in reverse engineering architectures that aren't natively supported by IDA, particularly those encountered in embedded systems, commercial firmware, and specialized computing hardware.

## Available Processor Modules

| Architecture | Description | Repository |
|---|---|---|
| **XMOS xCORE** | Event-driven multicore architecture used in embedded audio, USB, and real-time systems. | [xcore-ida](https://github.com/Mr-wolf-is-me/xcore-ida) |
| **TI C7x / C7000** | Advanced DSP architecture supporting parallel execution, vector operations, and specialized processing units. | [c7x-ida](https://github.com/Mr-wolf-is-me/c7x-ida) |
| **TI PRU / PRU-ICSS** | Deterministic real-time processors used in industrial communication, automation, and embedded control. | [pru-ida](https://github.com/Mr-wolf-is-me/pru-ida) |
| **AMD/Xilinx MicroBlaze** | Configurable soft-core RISC processor used inside FPGA-based systems. | [microblaze-ida](https://github.com/Mr-wolf-is-me/microblaze-ida) |
| **NVIDIA SASS** | Native NVIDIA GPU machine-code architecture with generation-specific instruction encodings. | [sass-ida](https://github.com/Mr-wolf-is-me/sass-ida) |

## About the Projects

Each architecture presents different reverse-engineering challenges, including:

- Instruction decoding and architecture-specific encoding formats.
- Register models, addressing modes, and operand representations.
- Control-flow analysis and instruction semantics.
- Parallel execution, DSP operations, and specialized instruction families.
- Architecture revisions and compatibility differences.

Development has involved studying vendor documentation, examining real binaries, using reference disassemblers, and experimentally analyzing instruction encodings.

The goal is to make these architectures more accessible to researchers working with IDA.

## Looking for the Next Architecture

I'm particularly interested in **obscure, unusual, or under-supported processor architectures** that appear in real-world firmware and executable binaries.

Good candidates typically have:

- An available instruction-set reference, preferably from the manufacturer.
- An assembler, compiler, or reference disassembler.
- Real firmware or executable binaries available for testing.
- No existing IDA processor module, or only limited support.

**Have you encountered an architecture that IDA doesn't support but you wish it did?**

Suggestions, technical discussions, and feedback are welcome.

Feel free to open a GitHub Discussion or Issue in the relevant repository.

---

*Developed out of curiosity about unusual processor architectures and the challenges of reverse engineering them.*
