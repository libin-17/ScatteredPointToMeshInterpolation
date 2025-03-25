# ScatteredPointToMeshInterpolation

## Overview

ScatteredPointToMeshInterpolation is a C-based utility designed to interpolate scattered data points onto a mesh grid. This tool is particularly useful in computational simulations where data from discrete points need to be mapped onto a continuous mesh for analysis or visualization.

## Features

- **Point-in-Cell (PIC) Interpolation:** Implements the PIC method to assign values from scattered data points to corresponding mesh cells.
- **Custom Input Generation:** Includes a utility to create input files with scattered data points for testing and demonstration purposes.

## Repository Structure

- `PIC_Interpolation.c`: Main source code implementing the PIC interpolation algorithm.
- `input_fileMaker.c`: Utility to generate input files containing scattered data points.
- `Test_input.bin`: Sample binary input file with scattered data points for testing.
- `Test_Mesh.out`: Sample output file demonstrating the interpolation results.
- `HPC_assignment.pdf`: Documentation detailing the methodology and implementation of the interpolation process.
- `README.md`: This file, providing an overview and guidance on using the project.

## Getting Started

### Prerequisites

- GCC compiler for compiling C programs.

### Compilation

To compile the source code files, use the following commands:

```bash
gcc -o PIC_Interpolation PIC_Interpolation.c -openmp
gcc -o input_fileMaker input_fileMaker.c
