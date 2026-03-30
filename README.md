# CAN Logger
<img width="1463" height="1309" alt="5b3f4bc4607f405ea5adb04bc922e155_T" src="https://github.com/user-attachments/assets/9520ca63-0f13-4def-9d17-c07ef67f6ade" />

A compact CAN bus logger and sniffer built for the HUGINN rocket. Built around the ESP32-C3 and SN65HVD230 transceiver, it sits on the CAN bus during ground support and pre-launch operations, streaming frames from the flight computer, sensor nodes, CAS board, and camera board over WiFi via MQTT for real-time monitoring.

## Overview

This board is designed for ground support and pre-launch monitoring of the HUGINN CAN bus. It passively sniffs CAN traffic and publishes decoded frames to an MQTT broker over WiFi, making it easy to verify system state, check sensor health, and monitor inter-board communication before launch.

## Hardware

| Component | Part |
|---|---|
| Microcontroller | ESP32-C3 |
| CAN Transceiver | SN65HVD230 |
| Power Input | 3.3V |

## Features

- CAN 2.0A/B frame capture
- Real-time publishing over WiFi via MQTT
- Passive monitoring, no interference with the CAN bus
- Compact form factor suitable for ground support equipment

## Monitored Systems

This board is intended to sniff traffic from the following Shingleback subsystems:

- Flight computer
- CAS board
- Camera board

## Status

Early prototype / bring-up phase. Not recommended for production use.

## License

MIT
