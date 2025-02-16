# Kriti-2025
# Electronics Project: Automated Rain-Detection and Wiper Control Mechanism

This project implements an automated system that detects rain intensity and dynamically adjusts the wiper speed accordingly. The design combines analog circuitry with microcontroller-based control to provide a robust solution for efficient wiper operation during varying rain conditions

# Features
# Automated Rain Detection:
Uses a rain sensor with an LM324 quad comparator circuit to detect four distinct water-level thresholds.

# One-Hot Encoding:
Ensures that only one digital output is active at a time for accurate level detection.

# Binary Weighted DAC:
Converts the one-hot encoded signal into a control voltage (V_con) using an inverting summing amplifier built with LM741 op amps.

# PWM Signal Generation:
A triangular waveform and comparator circuit generate a PWM signal at 5237 Hz, which adjusts the duty cycle based on rain intensity.

# Speed Indicator Circuit:
An Arduino UNO-based circuit controls a servo motor (for speed indication) and LED indicators to display the wiper speed.

# Motor Driver & Linkage Mechanism:
A high-side P-channel MOSFET (IRF9540N) drives a SE DC geared motor. A 3-bar linkage mechanism converts the motor’s 360° rotation into a 120° oscillatory motion of the wiper.
