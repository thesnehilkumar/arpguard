# ArpGuard

ArpGuard is a simple tool designed to safeguard your connectivity by monitoring ARP (Address Resolution Protocol) activities on a network interface.

## Version

Current version: 1.0

## Table of Contents

- [Features](#features)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Options](#options)

## Features

- Monitors ARP packets on a specified network interface.
- Detects possible ARP spoofing activities.
- Sends alerts when suspicious ARP activities are detected.

## Dependencies

- [libpcap](https://www.tcpdump.org/)
- [libnotify-bin](https://packages.debian.org/sid/libnotify-bin) (for alerts)

Ensure that these dependencies are installed before using the tool.

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/your-username/arpguard.git
cd arpguard
```

## Compile the code

```bash
gcc -o arpguard arpguard.c -lpcap
```

## Usage

```bash
./arpguard -h

-h or --help: Display help information.
-l or --lookup: Print available network interfaces.
-i or --interface: Specify the network interface to sniff on.
-v or --version: Display the tool's version information.

./arpguard -l

./arpguard -i <interface>
```

