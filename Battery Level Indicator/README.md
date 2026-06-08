# Battery Level Indicator

[cite_start]A simple hardware project that measures battery voltage and displays the charge level using a 10-LED bar graph, built around the LM3914 Integrated Circuit[cite: 184].

## Overview
[cite_start]This project uses the LM3914 IC to read an input voltage and light up a series of LEDs proportionally[cite: 289, 291]. [cite_start]In this specific setup, the circuit is calibrated to measure and display battery levels ranging from roughly 8.5V (1st LED turns on) up to 13V (all 10 LEDs on)[cite: 338].

## Components Used
* [cite_start]**IC:** LM3914 [cite: 186]
* [cite_start]**Display:** 10 LEDs [cite: 188]
* [cite_start]**Resistors:** 4.7kΩ, 18kΩ, 56kΩ [cite: 189]
* [cite_start]**Potentiometer:** 10kΩ Analog Potentiometer (for calibration) [cite: 190]
* [cite_start]**Misc:** Breadboard, connecting wires, battery/power supply [cite: 187, 191, 192]

## How It Works
[cite_start]The LM3914 IC contains 10 internal comparators[cite: 289]. [cite_start]We feed the battery's voltage into the IC's signal pin[cite: 289]. [cite_start]The IC compares this input against an adjustable reference voltage[cite: 289, 291]. [cite_start]As the battery voltage increases, it surpasses the reference voltage thresholds set for each pin, turning on the corresponding LEDs one by one[cite: 291, 325]. 

## Real-Life Applications
The core logic of this circuit can easily be adapted for:
* [cite_start]Charge indicators in power banks, electrical vehicles, and UPS systems[cite: 378, 380].
* [cite_start]Displaying physical factors from other analog sensors (like temperature, humidity, or sound intensity) by mapping their voltage output to the LED indicators[cite: 379].

## Precautions
* [cite_start]Ensure the voltage across the components doesn't exceed their limits (the LM3914 can withstand up to 35V)[cite: 382, 383].
* [cite_start]Always power off the circuit before modifying connections on the breadboard to avoid short circuits[cite: 385, 386].
