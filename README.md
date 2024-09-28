# Gate OS

## Desc

Gate OS is an experimental exokernel, drawing inspiration from the architectural designs proposed in the Aegis and Xok papers. The kernel is fully implemented in Rust and provides essential functionalities, including a basic shell, file system, networking stack, and process execution capabilities. The primary objective of Gate OS is to minimize the complexity between hardware and applications, particularly for high-throughput or short-lived tasks, where traditional operating system abstractions may be bypassed using mechanisms such as eBPF, XDP, or custom kernel drivers.

Exokernels remove resource management responsibilities from the kernel, delegating the optimization of system resources directly to applications. This design reduces the kernel’s role to the safe multiplexing of CPU time slices, memory pages, and network packets. Gate OS incorporates safe disk and network management through a minimal kernel downloading mechanism inspired by eBPF and uBPF. Additionally, ongoing development focuses on integrating static analysis of LLVM IR to ensure secure kernel downloads, eliminating the need for custom virtual machines.

## Compilation

## Run in QEMU

## Boot process

## References

- XoK: https://pdos.csail.mit.edu/archive/exo/
- Exokernel: https://en.wikipedia.org/wiki/Exokernel
- osDev: https://wiki.osdev.org/Expanded_Main_Page
- Moros: http://moros.cc/
