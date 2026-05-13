# 16-Bit Subtractor Design

A Digital Logic Design project that implements a 16-bit binary subtractor capable of subtracting two 16-bit binary numbers.

The circuit performs:

id="w9k2am" Output = A - B

where:
- A = 16-bit Minuend
- B = 16-bit Subtrahend

Outputs:
- Difference (16-bit)
- Borrow Out

## Project Objective

The objective of this project is to design and simulate a 16-bit subtractor circuit using digital logic components and arithmetic design principles.

## Features

- 16-bit binary subtraction
- Borrow propagation
- Difference output
- Borrow out detection
- Circuit simulation

## Components Used

- Full Subtractors
- XOR Gates
- AND Gates
- OR Gates
- NOT Gates

## Design Method

This project can be implemented using:

### Method 1: Ripple Borrow Subtractor
Using 16 Full Subtractors connected in sequence.

id="m4x7ql" FS0 → FS1 → FS2 → ... → FS15

### Method 2: 2’s Complement Subtraction
Using a 16-bit adder:

id="g8v5tr" A - B = A + (~B + 1)

Steps:
1. Invert B using NOT gates
2. Add 1 using Carry In = 1
3. Use 16-bit adder to generate result

## Truth Table (1-Bit Full Subtractor)

| A | B | Bin | Difference | Borrow |
|---|---|-----|------------|--------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 | 0 |

## Software Used

- Logisim
- Proteus
- Multisim
- Quartus

## Project Structure

bash id="r2n6yf" 16-bit-subtractor/ │ ├── design/ │   ├── circuit_design.png │   ├── truth_table.png │ ├── simulation/ │   └── subtractor_simulation.circ │ └── README.md 

## Example

Input:

id="f6p3dw" A = 0000000000001010 B = 0000000000000011

Output:

id="z1h8mu" Difference = 0000000000000111 Borrow Out = 0

## Applications

- Arithmetic Logic Unit (ALU)
- Processors
- Embedded systems
- Digital calculators

## Contributors

- Omar Ahmed

## Course

Digital Logic Design (DLD)

## License

This project is for educational purposes.
