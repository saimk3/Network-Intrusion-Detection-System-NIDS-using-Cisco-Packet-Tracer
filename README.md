# Network-Intrusion-Detection-System-NIDS-using-Cisco-Packet-Tracer
📘 Project Overview:
The report details the implementation of a Network Intrusion Detection System (NIDS) using Cisco Packet Tracer to simulate and monitor network traffic for unauthorized or suspicious activity.

🛡️ What is IDS?
An Intrusion Detection System (IDS) is a security tool that monitors networks or systems for malicious activities or policy violations.

Types of IDS:
NIDS (Network-based IDS)
HIDS (Host-based IDS)
PIDS (Protocol-based)
APIDS (Application Protocol-based)
Hybrid IDS

🧠 Background & Motivation:
The concept dates back to the 1980s (e.g., IDES model by Dorothy Denning).
Inspired by growing cybersecurity threats.
Chose IDS as a project to go beyond basic networking concepts and explore a more security-focused challenge.

🎯 Project Goals:
Create a secure and stable IDS that:
Detects suspicious network traffic.
Alerts the administrator.
Logs activity for analysis.
Use real networking simulation with multiple interconnected LANs.

🖥️ System Design & Tools Used:
Three separate networks were created using IPv4 addressing.
Devices included: PCs, laptops, servers (HTTP, FTP, SYSLOG), routers, switches.
Software Used: Cisco Packet Tracer.
Hardware Requirements: Basic modern PC specs.
Routing: Implemented using dynamic routing.
CLI Commands were extensively used to configure devices and IDS.

🔧 Implementation Steps:
Network Configuration:
Assigned IPs and connected 3 LANs using routers.
Configured servers with custom login/web pages.
IDS Configuration:
Implemented NIDS on Router0.
Used IPS Signature 2004 (ICMP Echo Request) to detect ping floods.
Enabled Syslog server to log alerts.

ip ips config location
ip ips signature-definition
event-action produce-alert
📊 Testing & Results:
Performed ping tests across networks to simulate intrusion.

IDS detected and logged ICMP packets (malicious pings).

Successfully alerted and logged suspicious activities via the Syslog server.

🚧 Challenges Faced:
IP address configuration.
Routing issues.
Command line syntax complexities.
Protocol configuration for servers.

🔮 Future Work:
Integrate Intrusion Prevention Systems (IPS).
Implement honeypot systems to trap attackers.

✅ Conclusion:
The project provided hands-on experience in network security.
IDS was successfully deployed and validated.
It demonstrated the potential for real-world intrusion detection in simulated environments.
