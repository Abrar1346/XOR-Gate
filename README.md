# MOSFET XOR Gate Project

## Project Overview
This project focuses on the design and implementation of an XOR gate using MOSFETs. The objective is to analyze the circuit's behavior, determine ideal sizing for the MOSFETs, and evaluate performance through static testing.

## Author
**Abrar Tamjid**  

## Circuit Design
The XOR gate circuit is implemented using MOSFETs based on the **MC14007** chip. The design requires **12 MOSFETs** (6 NMOS and 6 PMOS), utilizing the following approach:

- **Inversion Stage**: Each input passes through an inverter, requiring 4 MOSFETs.
- **AND Operation**: Implemented using 2 sets of NMOS and PMOS transistors.
- **OR Operation**: Achieved using an additional PMOS and NMOS pair.

![Circuit Schematic](images/XOR Schematic.png)

### Ideal Sizing
The ideal MOSFET sizing for the XOR circuit follows a **1:1 topology**, which ensures proper function while minimizing complexity. However, the high internal impedance of the MOSFETs in the **MC14007** chips may lead to suboptimal performance.

## Static Testing Results
Two tests were conducted to evaluate the performance of the XOR gate:

- **Test 1**: VL = -176 mV, VH = 4.21 V
- **Test 2**: VL = -151 mV, VH = 4.33 V

![Static Test 1](images/static_test_1.png)  
![Static Test 2](images/static_test_2.png)  

These results confirm that the circuit functions as expected, with slight variations in voltage levels that align with XOR gate logic.

## Files Included
- **Circuit Schematic**: Illustrates the XOR gate implementation.
- **Physical Circuit**: A visual representation of the built circuit.
- **Testing Results**: Data collected from static testing.

## Notes
- The use of MC14007 chips provides a practical implementation but may introduce minor inaccuracies due to impedance variations.
- Future improvements may involve optimizing MOSFET selection to reduce impedance effects
