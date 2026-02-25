# BCD-to-7-segment-decoder
A digital logic hardware project that implements a BCD (Binary Coded Decimal) to 7-Segment Decoder using combinational circuits and physical components. This project demonstrates how binary inputs (0000–1001) can be converted into decimal digits (0–9) and displayed on a 7-segment LED display. 

# Overview

The system takes a 4-bit binary input and converts it into the correct decimal digit using:
	•	Logic gates (AND, OR, NOT)
	•	A BCD-to-7-segment decoder circuit
	•	A counter for sequential operation
	•	A clock signal
	•	A 7-segment LED display
	•	Physical hardware components (7447 IC)

The project was implemented both:

✔ Digitally (circuit design & truth table)
✔ Physically (real hardware setup with IC 7447)

 
# Objectives
	•	Represent decimal digits (0–9) using 4-bit BCD input
	•	Design a complete truth table
	•	Implement the BCD circuit using combinational logic gates
	•	Build a counter system for sequential display (0 → 9 → 0 loop)
	•	Connect and test the hardware implementation

 
# System Architecture

 Step 1: Truth Table Design

Created the full mapping between:
	•	4-bit BCD inputs (A, B, C, D)
	•	7 output segments (a–g)

Each segment has a derived Boolean expression  ￼.

⸻

Step 2: BCD Logic Circuit

Implemented combinational logic using:
	•	AND gates
	•	OR gates
	•	NOT gates

Each output segment (a–g) is controlled by its logical expression.

⸻

Step 3: Counter Design

A 4-bit counter was added to:
	•	Automatically increment values
	•	Loop from 0 to 9
	•	Reset using a reset button
	•	Use a clock input to move between states  ￼

⸻

Step 4: Splitter

Since the counter outputs 4 bits together, a splitter was used to separate each bit and feed it into the decoder inputs individually.

⸻

Step 5: Hardware Integration

The physical hardware consists of:
	•	🔌 4-pin switch (input)
	•	🔢 7447 IC BCD Decoder
	•	💡 7-segment LED display
	•	🔁 Counter
	•	⏱ Clock
	•	🔄 Reset button
	•	⚡ Power & ground connections

The 7447 decoder converts 4-bit input into 7 output signals (a–g) which directly control the LED segments.

  
