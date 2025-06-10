# Design-and-Verification-of-a-1-3-Packet-Switching-Router-using-Verilog-HDL
This project implements a 1×3 packet-based router in Verilog, designed for use in digital communication systems where a single input stream must be routed to one of three output channels. The router decodes the packet header to determine the destination output port (port 0, 1, or 2) and forwards the payload accordingly. Each output has a dedicated FIFO buffer for temporary storage, supporting concurrent queuing and delivery.

The design supports features such as packet validation, error detection via parity, busy signal handling, and read-enable-based output control. The routing logic is modular and synchronous with clock-driven operation, making it ideal for FPGA implementation.

The system is developed, simulated, and verified using Xilinx ISE with a robust Verilog testbench. The testbench covers different packet lengths, destinations, and includes corner cases to ensure correctness. It uses tasks to emulate real-time packet generation and FIFO interactions, and generates VCD waveforms for detailed analysis.

This project serves as a solid foundation for understanding basic NoC (Network-on-Chip) concepts, buffering strategies, and packet-based communication in hardware. It is a great educational exercise in RTL design, synthesis, and verification using Verilog and Xilinx tools.
