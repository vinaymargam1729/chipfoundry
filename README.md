# Edge Detector Peripheral for Microwatt

## Overview

This project implements a **memory-mapped Edge Detector peripheral** in Verilog, designed for direct integration with the [Microwatt](https://github.com/antonblanchard/microwatt) open-source POWER CPU core. The peripheral monitors multiple input signals, detects rising and falling edges, latches event status, and can generate interrupts for prompt CPU response. It offers a highly reusable and practical digital IC function for embedded and open hardware systems.

---

## Key Features

- Monitors 4 digital input channels in real time
- Detects and latches rising and falling edge events per channel
- Memory-mapped register interface for communication with the Microwatt CPU
- Configurable interrupt signal to the CPU on edge event detection
- Status flags for each input, which can be cleared by software
- Includes a self-checking Verilog testbench for comprehensive verification

---

## Integration with Microwatt

- Exposed as a memory-mapped peripheral within the SoC address space
- Status and control registers accessible by the CPU for configuration and event handling
- Example software demonstrates polling and interrupt-driven edge event processing

---

## Usage Scenarios

- Frequency and pulse width measurement
- User input (button/key event) detection
- Instrumentation, timing, and control systems
- General event capture in digital SoC platforms

---

## Deliverables

- Verilog RTL code for the edge detector peripheral
- Memory-mapped register and bus interface implementation
- Testbench verifying all edge cases and interrupt features
- Documentation for hardware and software integration
- Example C/assembly for Microwatt-managed event handling
- Demo video or simulation screenshots illustrating correct operation

---

## License

This project is open source and distributed under the [MIT License](LICENSE).

---

## Contributors

- [Margam Vinay](margam.vinay2025@vitstudent.ac.in)
