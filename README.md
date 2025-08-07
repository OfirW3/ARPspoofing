# ARP Spoofing Demonstration Script

This project provides a Python script designed to demonstrate a fundamental vulnerability in the ARP (Address Resolution Protocol). The script performs an ARP spoofing (Man-in-the-Middle) attack using the `scapy` library to illustrate how easily ARP can be exploited on local networks that lack proper security controls.

## Disclaimer

This tool is intended strictly for educational and authorized security testing purposes. Unauthorized use of this script on networks you do not own or have explicit permission to test may violate local or international laws. The author assumes no responsibility for any misuse or damages caused.

## Overview

ARP (Address Resolution Protocol) is responsible for mapping IP addresses to MAC addresses on local networks. It is inherently vulnerable because it lacks authentication. This allows attackers to impersonate devices by sending forged ARP responses, potentially redirecting or intercepting network traffic.

This script demonstrates that vulnerability by:

- Sending forged ARP replies to both a target machine and the network gateway
- Redirecting network traffic through the attacker's machine (Man-in-the-Middle)
- Optionally restoring original ARP mappings upon termination

## Features

- Lightweight and portable single-file implementation
- Uses `scapy` for packet crafting and transmission
- Automatically restores ARP tables upon exit
- Helps visualize the impact of ARP spoofing on insecure networks

## Requirements

- Python 3.x
- Scapy

Install Scapy with:

```bash
pip install scapy

```bash
pip install -r requirements.txt
