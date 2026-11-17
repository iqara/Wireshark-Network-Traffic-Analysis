# 🔐 Network Traffic Analysis & Security Monitoring Using Wireshark

## 📌 Project Overview

This cybersecurity project demonstrates practical network traffic analysis and basic security monitoring using Wireshark.

The project focuses on capturing network packets, analyzing communication protocols, investigating network behavior, and identifying traffic patterns that may require further security investigation.

The investigation was performed in a Windows 11 environment using Wireshark.

## 🎯 Project Objectives

- Capture and inspect network packets.
- Analyze TCP and UDP communication.
- Identify the TCP three-way handshake.
- Investigate DNS queries and responses.
- Examine HTTPS/TLS encrypted communication.
- Identify TCP retransmissions.
- Investigate DNS resolution errors.
- Analyze network statistics and conversations.
- Document findings in a cybersecurity investigation report.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| Wireshark | Network packet capture and analysis |
| Npcap | Packet capture driver |
| Windows 11 | Investigation environment |
| Command Prompt | Generating DNS queries |
| Visual Studio Code | Project documentation |

## 🔬 Investigation Methodology

### 1. Network Traffic Capture

Captured network traffic using Wireshark and examined packet details, including source and destination addresses, protocols, ports, and packet information.

### 2. TCP Analysis

Analyzed TCP communication and identified the three-way handshake:

1. SYN
2. SYN-ACK
3. ACK

### 3. UDP Analysis

Examined UDP packets and their transport-layer header information.

### 4. DNS Analysis

Investigated DNS queries and responses to understand domain name resolution.

### 5. HTTPS/TLS Analysis

Examined TLS traffic to understand encrypted network communication.

### 6. Security Investigation

Investigated TCP retransmissions, DNS resolution errors, protocol distribution, and network conversations.

## 🔎 Wireshark Display Filters

| Filter | Purpose |
|---|---|
| `tcp` | Display TCP packets |
| `udp` | Display UDP packets |
| `dns` | Display DNS traffic |
| `tls` | Display TLS traffic |
| `tcp.port == 443` | Display TCP traffic using port 443 |
| `tcp.flags.syn == 1 && tcp.flags.ack == 0` | Identify initial TCP SYN packets |
| `tcp.analysis.retransmission` | Identify TCP retransmissions |
| `dns.flags.rcode == 3` | Identify DNS NXDOMAIN responses |

## 📊 Findings

### TCP Communication

Successfully identified and analyzed the TCP three-way handshake.

### UDP Communication

Observed UDP packets and examined their protocol characteristics.

### DNS Traffic

Identified DNS queries and responses.

No DNS NXDOMAIN responses were observed in the analyzed capture.

### HTTPS/TLS Traffic

Identified TLS communication and examined encrypted network traffic.

### TCP Retransmissions

TCP retransmissions were observed during the investigation.

These may result from packet loss, network congestion, or delayed acknowledgments.

The observations did not establish that a cyberattack occurred.

### Network Statistics

Used Wireshark's Protocol Hierarchy and Conversations features to examine network communication patterns.

## 📸 Project Screenshots

The `screenshots` folder contains evidence of the investigation, including:

- Initial network packet capture
- TCP three-way handshake
- UDP packet analysis
- DNS query and response analysis
- HTTPS/TLS traffic analysis
- TCP retransmission investigation
- DNS NXDOMAIN investigation
- Protocol Hierarchy statistics
- Network Conversations statistics

Screenshots were reviewed to avoid publicly exposing sensitive network information.

## 🛡️ Security Recommendations

1. Monitor network traffic for unusual communication patterns.
2. Investigate persistent TCP retransmissions and connectivity problems.
3. Review unexpected DNS resolution failures.
4. Use encrypted protocols such as HTTPS.
5. Keep operating systems and network security tools updated.
6. Apply appropriate firewall and network access controls.

## 📚 Skills Demonstrated

- Network packet capture
- TCP/IP protocol analysis
- DNS traffic investigation
- HTTPS/TLS analysis
- Network troubleshooting
- Basic security monitoring
- Wireshark display filtering
- Cybersecurity reporting

## 📄 Security Analysis Report

A detailed investigation report is available in the `reports` folder.

## ⚠️ Ethical and Privacy Considerations

This project was conducted for educational and defensive cybersecurity purposes.

Network traffic was analyzed in an authorized environment.

Original packet captures are not included in the public repository to reduce the risk of exposing sensitive information.

## 🏁 Conclusion

This project strengthened practical skills in network traffic analysis, protocol inspection, and basic security monitoring.

The investigation provided experience using Wireshark to examine normal network communication and identify patterns that may require further investigation.

These skills are relevant to entry-level cybersecurity and Security Operations Center (SOC) analyst roles.
