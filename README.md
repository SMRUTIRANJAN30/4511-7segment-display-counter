# 4511-7segment-display-counter
BCD to 7-Segment Display using CD4511 IC with Common Cathode display. Simulated in Proteus and Tinkercad showing digits 0–9 


# BCD to 7-Segment Display using CD4511 IC (Common Cathode)

## Project Overview

This project demonstrates how to display decimal numbers (0–9) on a **7-segment display** using the **CD4511 BCD to 7-segment decoder/driver IC**.

The circuit accepts a **4-bit BCD input** and converts it into the correct signals required to drive a **common cathode 7-segment display**.

This project was simulated using:

* **Proteus**
* **Tinkercad**

The circuit verifies the output by displaying numbers from **0 to 9**, and a demonstration input of **543** using three displays.

---

# Components Required

* CD4511 BCD to 7-Segment Decoder IC
* Common Cathode 7-Segment Display
* 330Ω Resistors (7 pieces)
* Push Buttons / Logic Inputs
* Power Supply (5V)
* Connecting Wires

---

# Pin Description of CD4511

| Pin | Name | Function       |
| --- | ---- | -------------- |
| 1   | B    | BCD Input      |
| 2   | C    | BCD Input      |
| 3   | LT   | Lamp Test      |
| 4   | BI   | Blanking Input |
| 5   | LE   | Latch Enable   |
| 6   | D    | BCD Input      |
| 7   | A    | BCD Input      |
| 8   | GND  | Ground         |
| 9   | e    | Segment output |
| 10  | d    | Segment output |
| 11  | c    | Segment output |
| 12  | b    | Segment output |
| 13  | a    | Segment output |
| 14  | g    | Segment output |
| 15  | f    | Segment output |
| 16  | VDD  | +5V Supply     |

---

# Circuit Connections

### Power Supply

VDD (Pin 16) → +5V
GND (Pin 8) → Ground

### Control Pins

LT (Pin 3) → HIGH
BI (Pin 4) → HIGH
LE (Pin 5) → LOW

### BCD Inputs

A → Pin 7
B → Pin 1
C → Pin 2
D → Pin 6

### Segment Outputs

Connect CD4511 outputs to 7-segment through **330Ω resistors**

| CD4511 Pin | Segment |
| ---------- | ------- |
| 13         | a       |
| 12         | b       |
| 11         | c       |
| 10         | d       |
| 9          | e       |
| 15         | f       |
| 14         | g       |

### Display Type

Use **Common Cathode 7-Segment Display**

Common Cathode → Ground

---

# BCD Truth Table

| Decimal | D | C | B | A |
| ------- | - | - | - | - |
| 0       | 0 | 0 | 0 | 0 |
| 1       | 0 | 0 | 0 | 1 |
| 2       | 0 | 0 | 1 | 0 |
| 3       | 0 | 0 | 1 | 1 |
| 4       | 0 | 1 | 0 | 0 |
| 5       | 0 | 1 | 0 | 1 |
| 6       | 0 | 1 | 1 | 0 |
| 7       | 0 | 1 | 1 | 1 |
| 8       | 1 | 0 | 0 | 0 |
| 9       | 1 | 0 | 0 | 1 |

The CD4511 decodes these BCD inputs and activates the correct segments.

---

# Example Demonstration (Displaying 543)

Three CD4511 ICs and three 7-segment displays can be used.

| Digit | BCD Input |
| ----- | --------- |
| 5     | 0101      |
| 4     | 0100      |
| 3     | 0011      |

So the display shows:

543

---

# Simulation Tools

### Proteus

Proteus was used to design and simulate the circuit.

Files included:

* `.dsn` schematic file
* `.pdsprj` project file

---

### Tinkercad

The circuit was also simulated using Tinkercad.

Simulation link:
Paste your Tinkercad share link here.

Example:
https://www.tinkercad.com/things/example

---

# Output

The 7-segment display correctly shows digits **0–9** depending on the BCD input.

Example output:

0
1
2
3
4
5
6
7
8
9

And demonstration value:

543

---

# Applications

* Digital clocks
* Counters
* Calculators
* Digital measurement instruments
* Embedded system displays

---

# Author

Smrutiranjan Sahoo
B.Tech Electronics and Communication Engineering

Interested in:

* VLSI Design
* Digital Electronics
* IoT Projects
* Semiconductor Technology

---

# License

This project is open source and free to use for educational purposes.
