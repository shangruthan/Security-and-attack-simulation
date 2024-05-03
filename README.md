# Network Traffic Analysis and Security Assessment

## Overview
This project aims to conduct a comprehensive analysis of network traffic utilizing manual classification techniques based on protocol headers. The focus is on identifying normal network behavior and potential security threats, including various cyber attacks such as SYN flood attacks and Denial of Service (DoS) attacks. The project involves refining existing methodologies, collecting live network traffic data using Wireshark, and conducting statistical analysis to enhance understanding and proactive management of network security risks.

## Objectives
1. Refinement of existing methodologies to focus on using protocol headers for manual classification and analysis of network traffic.
2. Capture live network traffic using Wireshark, targeting diverse protocols and traffic patterns to represent both normal behavior and potential threats.
3. Manual analysis of captured packets to extract protocol headers and classify each packet into predefined types.
4. Aggregation of classified packets for statistical analysis to determine distribution and characteristics of different protocol types and analyze the impact of attack simulations.
5. Documentation of experimental setup, procedures, findings, and insights gained from the analysis.

## Techniques and Tools
- **Wireshark:** Utilized for live packet capture and analysis.
- **TCP Stream Analysis:** Followed TCP streams to visualize communication between devices.
- **Attack Simulations:** Simulated various cyber attacks such as SYN flood and DoS attacks for analysis.

## Attack Simulations
### SYN Flood Attack
A SYN flood attack was simulated using the hping3 tool to flood a victim server with SYN packets. The captured traffic revealed a significant influx of SYN packets directed towards the victim server, overwhelming its resources and disrupting normal operation.

### DoS Attack
A Denial of Service (DoS) attack was simulated using the macof tool to flood a device's switch with MAC addresses, generating excessive network traffic. Analysis showed repeated requests, indicating a standard network DoS attack, and packets with fake source and destination IP addresses, characteristic of a Distributed Denial of Service (DDoS) attack.

## Results and Interpretation
- No findings of brute source or other attacks were observed in normal network traffic.
- Detection of duplicate requests in the threat pcap file raised concerns about security threats.
- The SYN flood and DoS attack simulations demonstrated the potential impact on network traffic and the importance of robust defense mechanisms.

## Conclusion
This project showcased critical thinking skills in refining objectives, collecting and analyzing network traffic data, and identifying potential security threats. Emphasis was placed on attack simulations to understand their impact and bolster network security defenses. Continuous monitoring, analysis, and response are essential to safeguard against potential cyber threats and attacks.
