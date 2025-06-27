# Firewall_rules

## 🎯 Objective
Block and test inbound traffic on port 23 (Telnet) using Windows Defender Firewall, verify rule enforcement via testing, and document findings for review.

## ⚙️ Tools & Environment
- Windows 10/11
- Windows Defender Firewall with Advanced Security
- Telnet Client (enabled via Windows Features)
- Command Prompt (CMD)

## 🧭 Task Workflow

1. **Opened Windows Firewall Management**
   - Accessed via `wf.msc` (Run dialog)

2. **Created an Inbound Rule**
   - Protocol: TCP
   - Port: 23 (Telnet)
   - Action: Block the connection
   - Profiles: Domain, Private, Public

3. **Tested the Firewall Rule**
   - Enabled Telnet Client
   - Command Used:
     ```cmd
     telnet localhost 23
     ```
   - Result: Connection blocked as expected ✅

4. **Removed the Rule After Testing**
   - Rule `Block_Telnet_23` was deleted to restore the system’s original state.

## 🧠 Key Concepts Illustrated
- Inbound vs. Outbound Firewall Rules
- Telnet as a vulnerable service (port 23)
- Role of firewalls in filtering traffic based on port/protocol
- Security best practices in system hardening.

## ✅ Outcome
Successfully implemented and tested a custom firewall rule on Windows. This task demonstrates system-hardening skills and understanding of traffic filtering—a key component of defensive cybersecurity.

