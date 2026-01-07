# Low-Level Socket Protocols

A collection of bare-metal networking implementations using **Berkeley Sockets**.
This project demonstrates the fundamental differences between **TCP** (Reliable, Connection-oriented) and **UDP** (Fast, Connection-less) protocols through implementation in both **C** and **Python**.

> **Status:** Educational / Reference

## 🚀 Overview

| Protocol | Type | Key Characteristics | Implemented In |
| :--- | :--- | :--- | :--- |
| **TCP** | Stream | Reliable, Ordered, Error-Checked | C |
| **UDP** | Datagram | Fast, Low Latency, No Guarantee | C, Python |

## 📂 Project Structure
```text
.
├── TCP/
│   ├── tcpServer.c      # The listener (Server)
│   └── tcpClient.c      # The sender (Client)
├── UDP/
│   ├── udpServer.c      # C implementation of UDP Server
│   ├── udpClient.c      # C implementation of UDP Client
│   ├── udpServer.py     # Python implementation (Cross-language test)
│   └── udpClient.py     # Python implementation
├── Makefile             # Build script
└── README.md            # Documentation
```

## 🧠 Key Concepts Learned
- **Socket Creation:** `socket(AF_INET, ...)`
- **Binding:** Associating a socket with a specific Port/IP.
- **Listening/Accepting:** The specific workflow for TCP connection establishment.
- **Datagrams:** Sending discrete packets (`sendto`) vs streams (`send`).

## 🤝 Contribution
Feel free to add implementations in other languages (Rust, Go) to compare socket APIs!