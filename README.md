# Quantum Random Number Generator

This program generates a random number of 2^x-bits in length using x qubits. Each qubit can represent 2 bits of randomness. For example:
- 2 qubits = 4-bit random value
- 3 qubits = 8-bit random value (1 byte)
- 4 qubits = 16-bit random value (1 short, int16)
- 5 qubits = 32-bit random value (int32)

## How It Works
1. Determine the number of bits required for the maximum integer value: log2(n) + 1
2. Place the required number of qubits into superposition.
3. Measure the qubits to collapse them into classical bits.
4. Use the measured bits to construct the random number.

## Usage
Simply run the program, and it will output a random number. The number of qubits needed for the program is also displayed.

## Example Output
Number of qubits needed is: 6
[7724042831177568984, 13485200797250650711, 16908658522367577024, ...]

## Dependencies
- Qiskit
- configparser

## Author
Kevin Wong, Cal Poly Pomona, 3801 W Temple Avenue, Pomona, CA 91768
