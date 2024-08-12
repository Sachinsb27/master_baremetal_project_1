Project Overview


This project was developed as part of a hackathon challenge, aiming to interface an LDR with an embedded system and control a USER LED based on light intensity.

Problem Statement


The task involves:

Connecting an LDR to the analog pin P2.1.
Configuring P2.1 as an analog input.
Setting up the ADC peripheral to deliver a 12-bit output with a sampling frequency of 1 MHz.
Implementing continuous ADC conversion using the polling method.
Controlling a USER LED connected to digital pin P3.4, which turns ON when the ADC value corresponds to a voltage greater than 1.5V.

This implementation considers the following:
0V produces an ADC result of 0.
5V produces an ADC result of 4095.
The actual voltage (V) is calculated as:
V = ADC_Result * (5 / 4096).
