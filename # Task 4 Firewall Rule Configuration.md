# Task 4: Firewall Rule Configuration

## 🔒 Objective:
Use firewall settings to block and allow specific ports, test their effect, and understand traffic filtering.

---

## 🪟 Platform Used:
**Windows 10**  
**Firewall Tool:** Windows Defender Firewall with Advanced Security  
**Additional Tool:** Telnet (installed manually)

---

## 🔧 Steps Followed:

### 1. Opened the Firewall Configuration Tool
- Searched for **"Windows Defender Firewall with Advanced Security"** from Start Menu.

### 2. Listed Current Rules
- Explored **Inbound** and **Outbound** rules.

### 3. Blocked Port 23 (Telnet)
- Created a new inbound rule:
  - Port: TCP, Port number: 23
  - Action: Block the connection
  - Applied to: Domain, Private, Public
  - Name: `Block Telnet Port 23`

### 4. Tested Block Rule
- Enabled **Telnet** using:
  ```bash
  dism /online /Enable-Feature /FeatureName: TelnetClient


