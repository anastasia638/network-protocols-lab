# Network Protocols Lab

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![Networking](https://img.shields.io/badge/Networking-TCP%2FUDP-green) ![Status](https://img.shields.io/badge/Status-Active-brightgreen)

> Hands-on implementations of core network protocols and socket programming concepts, developed as part of coursework in Computer Networks at Université Lyon 1.

## Table of Contents
- [Overview](#overview)
- [Labs](#labs)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Author](#author)

## Overview

This repository contains practical lab exercises covering fundamental networking concepts. Each lab focuses on a specific protocol or networking concept, with working Python implementations and analysis reports.

## Labs

| Lab | Topic | Description |
|-----|-------|-------------|
| `lab01/` | TCP Server/Client | Bidirectional communication with persistent connections |
| `lab02/` | UDP Datagram Socket | Connectionless messaging and packet loss simulation |
| `lab03/` | HTTP Request Parser | Manual HTTP/1.1 request parsing and response generation |
| `lab04/` | Port Scanner | TCP SYN scanning over a given IP range |
| `lab05/` | Wireshark Analysis | Packet capture analysis — DNS, ARP, TCP handshake |

## Technologies

- **Language:** Python 3.x
- **Libraries:** `socket`, `threading`, `struct`, `scapy`
- **Tools:** Wireshark, Netcat, tcpdump
- **OS:** Linux (Ubuntu)

## Project Structure

```
network-protocols-lab/
├── lab01-tcp/
│   ├── server.py
│   └── client.py
├── lab02-udp/
│   ├── udp_server.py
│   └── udp_client.py
├── lab03-http/
│   └── http_parser.py
├── lab04-scanner/
│   └── port_scanner.py
├── lab05-wireshark/
│   └── analysis_report.md
└── README.md
```

## How to Run

```bash
# Clone the repository
git clone https://github.com/anastasia638/network-protocols-lab.git
cd network-protocols-lab

# Run TCP server/client (open two terminals)
python3 lab01-tcp/server.py
python3 lab01-tcp/client.py

# Run port scanner
python3 lab04-scanner/port_scanner.py --target 127.0.0.1 --range 1-1024
```

## Skills Demonstrated

- **Socket Programming:** TCP and UDP socket creation, binding, and communication
- **Protocol Analysis:** Reading and interpreting packet captures in Wireshark
- **Multi-threading:** Handling concurrent connections in the TCP server
- **Low-level Networking:** Manual header construction with `struct`

## Author

**Meriem Silmi** — Computer Science Student, France  
Licence 3 | Université Lyon 1
