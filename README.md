## Buck Converter (DC-DC Step-Down)

## Overview
This project demonstrates the design, simulation, and hardware implementation of a step-down DC-DC converter. It uses Pulse Width Modulation (PWM) to regulate output voltage by controlling the duty cycle of a switching MOSFET. The output was tested by driving a DC motor and LED lights under varying load conditions.

## Specifications
Input Voltage: 9V – 25V
Output Voltage: 1V – 24V (adjustable via potentiometer)
Output Current: up to 1.5A
Measured Efficiency: ~62.71%
Output formula: Vout = D × Vin (where D = duty cycle)

## Working Principle
The 555 timer generates a PWM square wave that drives the IRFZ44N MOSFET. When the MOSFET switches ON, current flows through the inductor to the load, storing energy in its magnetic field. When it switches OFF, the inductor releases stored energy through the freewheeling diode, maintaining continuous current to the load. The LC filter smooths the output into stable DC.

## Results
1. Successfully stepped down input voltages across the full range
2. Stable operation under different loads (motor and LEDs)
3. Mean input voltage: 15.5V → Mean output voltage: 9.72V
4. Power dissipated: 8.67W

## Team
Ayesha Mohsin · Laveeza Fatima · Fatima Habib · Ramisa Irum · Hafsa Sultan
