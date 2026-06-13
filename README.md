# Wireshark HTTP Traffic Analysis

## Overview

This project demonstrates packet-level network traffic analysis using Wireshark and TShark. The objective is to capture network packets, filter HTTP traffic, inspect packet details, analyze the TCP three-way handshake, and understand how network communication occurs.

---

## Objectives

* Capture live network traffic using Wireshark
* Filter HTTP packets
* Analyze HTTP request packets
* Study TCP three-way handshake
* Follow TCP streams
* Perform command-line packet analysis using TShark

---

## Tools Used

* Wireshark
* TShark
* Windows Command Prompt

---

## Project Workflow

### 1. Start Packet Capture

* Opened Wireshark
* Selected active Wi-Fi interface
* Started live packet capture

### 2. Filter HTTP Traffic

Applied the following filter:

```text id="a6v5bm"
http
```

This displayed only HTTP packets.

---

### 3. Analyze HTTP Request Packet

Expanded:

* Internet Protocol Version 4
* Transmission Control Protocol
* Hypertext Transfer Protocol

Observed:

* Request Method
* Host Header
* User-Agent

---

### 4. Analyze TCP Handshake

Observed the TCP three-way handshake:

* SYN
* SYN-ACK
* ACK

This establishes communication between client and server.

---

### 5. Follow TCP Stream

Used:
Right Click → Follow → TCP Stream

This displayed the complete communication between systems.

---

### 6. TShark Analysis

Commands used:

```bash id="u8tvmo"
tshark -D
```

```bash id="0wg1yh"
.\tshark.exe -r "..\capture.pcapng"
```

```bash id="xlgcpr"
.\tshark.exe -r "..\capture.pcapng" -Y http
```

---

## Screenshots Included

1. Wireshark Capture Started
2. HTTP Filter Applied
3. HTTP Request Packet Details
4. TCP Three-Way Handshake
5. Follow TCP Stream
6. TShark Command Output

---

## Learning Outcomes

* Understood packet-level communication
* Learned TCP connection establishment
* Performed HTTP traffic inspection
* Used packet filtering techniques
* Gained experience with Wireshark and TShark

---

## Conclusion

This project successfully demonstrated how network traffic can be captured and analyzed using Wireshark and TShark. It provided practical understanding of HTTP communication, TCP handshakes, and packet-level traffic inspection used in cybersecurity and network analysis.
