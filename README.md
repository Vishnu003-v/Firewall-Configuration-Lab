# Windows Defender Firewall Configuration Lab

## Overview

This lab demonstrates how to configure and manage firewall rules using **Windows Defender Firewall with Advanced Security**. The exercise includes viewing existing firewall rules, blocking Telnet traffic on Port 23, testing the rule, allowing SSH on Port 22, and restoring the firewall configuration by removing the temporary rule.

---

## Objectives

- Open Windows Defender Firewall.
- View existing inbound firewall rules.
- Block inbound traffic on Port 23 (Telnet).
- Test the firewall rule.
- Allow inbound SSH traffic on Port 22.
- Remove the temporary block rule.
- Understand how firewall filters network traffic.

---

## Software Used

- Windows 10/11
- Windows Defender Firewall with Advanced Security
- Windows PowerShell

---

## Procedure

1. Opened **Windows Defender Firewall with Advanced Security** using `wf.msc`.
2. Viewed existing inbound firewall rules.
3. Created a new inbound rule to block TCP Port 23.
4. Tested the blocked port using:

```powershell
Test-NetConnection localhost -Port 23
```

5. Created an inbound rule to allow TCP Port 22 (SSH).
6. Deleted the temporary Telnet block rule.

---



## Result

The Windows Defender Firewall was successfully configured to block Telnet traffic on Port 23 and allow SSH traffic on Port 22. The firewall rule was verified using PowerShell, and the temporary blocking rule was removed after testing.

---

## Conclusion

Windows Defender Firewall provides an effective mechanism for controlling network traffic by allowing or blocking connections based on predefined rules. Proper firewall configuration enhances system security by preventing unauthorized access while permitting legitimate services.
