 # wireshark-syn-scan-analysis
Wireshark-based analysis of TCP SYN scan traffic generated using Nmap in a controlled lab environment.

## Overview
This project demonstrates how TCP SYN scan activity can be identified and analyzed using Wireshark by examining network traffic patterns generated during an Nmap scan.

## Lab Setup
Attacker:- Kali Linux  
Target:- Metasploitable  
Tool:- Wireshark  

## Procedure
Network traffic capture was started in Wireshark before initiating the scan.  
A TCP SYN scan was generated from Kali Linux using Nmap against the target system.  
Captured traffic was filtered to focus on TCP SYN packets.  
Packet behavior and connection attempts were analyzed to identify scan characteristics.

## Findings
Multiple TCP SYN packets were observed without full TCP handshake completion.  
Repeated connection attempts to different ports were detected from a single source IP.  
Traffic patterns matched typical TCP SYN scan behavior.

## Skills Demonstrated
Network traffic analysis  
TCP SYN scan identification  
Wireshark filtering and packet inspection  
SOC-style traffic investigation

## Screenshots
All screenshots related to the traffic capture and analysis are included in the screenshots directory.

## Disclaimer
This project was conducted in a controlled lab environment for educational purposes only.

## SOC Analyst Perspective
If SYN scan traffic was detected:
- I would analyze packet flags and scan patterns.
- Identify whether the scan is internal or external.
- Correlate findings with IDS or firewall alerts.
- Escalate as reconnaissance if scans are repeated.

