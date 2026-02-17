# PortScan_LocalMachine

BASIC PORT SCANNING (Nmap)


Name : Dehiwattage Kavindu Nishitha Fernando

Role : SOC Analyst (Lab Project)

Date : 16/02/2026


This project demonstrates foundational understanding of network reconnaissance techniques through practical implementation of TCP port scanning using Nmap. A controlled scan was performed against the local host machine to identify open services and observe how reconnaissance traffic is generated. The lab provides insight into attacker behavior during the discovery phase and builds networking knowledge relevant to SOC detection and security monitoring.

________________________________________

Project Objective

The objective of this lab was to:

•	Understand how TCP port scanning works

•	Identify open ports and exposed services

•	Analyze TCP handshake behavior

•	Observe how reconnaissance activity is generated

•	Relate scanning behavior to security monitoring concepts

________________________________________

Environment Setup


Component	Description

Tool Used:	Nmap

Operating System:	Windows


Target:	Localhost 

Scan Type:	TCP SYN Scan

All scanning was conducted in a controlled lab environment on my own machine.

________________________________________

 Methodology

* Installation

Nmap was installed using the official Windows installer package.

* Basic Scan Execution

Initial scan performed:
nmap 127.x.x.x

This scanned the top 1000 common TCP ports.

* Extended Port Range Scan:
nmap -p 1-300 127.x.x.x

This simulated reconnaissance activity across a broader port range.

________________________________________

Technical Explanation

Nmap performs TCP scanning by:

1.	Sending TCP SYN packets to target ports

2.	Analyzing responses:

   o	SYN-ACK → Port is open

   o	RST → Port is closed

   o	No response → Port is filtered

This technique is commonly used during the reconnaissance phase of cyber attacks.
________________________________________

Findings

•	Identified open ports running local services

•	Observed how rapid sequential port requests are generated

•	Understood how scanning creates identifiable network patterns



________________________________________

Security Relevance

Port scanning aligns with:
MITRE ATT&CK

Technique: T1046 – Network Service Discovery

Tactic: Discovery

Port scanning is often an early-stage reconnaissance technique preceding exploitation attempts.
________________________________________

Conclusion

This lab strengthened foundational knowledge of:

   •	TCP/IP behavior

   •	Network reconnaissance techniques

   •	Service exposure identification

   •	How attackers enumerate systems

The project builds networking understanding necessary for both offensive security and SOC detection roles.

