# Verilog Ethernet ML605 Example Design

## Introduction

This example design targets the Xilinx ML605 FPGA board.

The design by default listens to UDP port 1234 at IP address 192.168.1.128 and
will echo back any packets received.  The design will also respond correctly
to ARP requests.  

FPGA: XC6SlX45-2CSG324
PHY: Marvell M88E1111

## How to build

Run make to build.  Ensure that the Xilinx ISE toolchain components are
in PATH.  

## How to test

Run make program to program the ML605 board with the Xilinx Impact software.
Then run netcat -u 192.168.1.128 1234 to open a UDP connection to port 1234.
Any text entered into netcat will be echoed back after pressing enter.  


