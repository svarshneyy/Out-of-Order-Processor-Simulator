# Out-of-Order Processor Simulator (C++)

Three projects from **ECE 721: Advanced Microarchitecture** at NC State University (Spring 2026). Together they build and extend a cycle-level simulator of a superscalar, out-of-order RISC-V processor.

## Results at a glance

| Project | Result |
|---|---|
| Register renamer | Matched the reference simulator on every validation run |
| Out-of-order pipeline | Integrated into the full simulator; became the base for the value prediction project |
| Value prediction | Matched the reference simulator on every validation run, then raised harmonic mean IPC from **1.658 to 2.035 (+22.7%)** across 15 benchmarks under a 32 KB storage budget |

## Projects

### Register renamer

Built the register renaming unit of an out-of-order core: physical register allocation, in-order commit tracking, and recovery from branch mispredictions and exceptions.

### Out-of-order pipeline

Completed the core pipeline stages of the simulator, from rename through retire, and integrated the register renamer.

### Value prediction (team project with Iman Khan)

Added a stride value predictor to the pipeline, covering prediction, verification, training and misprediction recovery. Then tuned it for a class-wide IPC competition with a fixed predictor storage budget.

## Tools

C++, a cycle-level RISC-V superscalar simulator, and an HPC cluster for benchmark runs.

## Author

Sanchit Varshney
