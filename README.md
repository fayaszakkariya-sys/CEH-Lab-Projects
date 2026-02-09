# Project: Vulnerability Assessment of Metasploitable 2

## Objective
To demonstrate the end-to-end process of identifying and exploiting a network vulnerability in a controlled lab environment.

## Lab Environment
* **Attacker OS:** Kali Linux (VirtualBox)
* **Target OS:** Metasploitable 2 (VirtualBox)
* **Network:** Host-Only Private Network

## Phase 1: Reconnaissance
I used **Nmap** to scan the target for open ports and services.
* **Findings:** Identified Port 21 (FTP) running vsftpd 2.3.4.

![Nmap Scan Results](open_ports_scan.pdf)

## Phase 2: Exploitation
Using the **Metasploit Framework**, I targeted the `vsftpd_234_backdoor` vulnerability.
* **Result:** Successfully gained a root shell, allowing full command execution on the target.

## Conclusion
This project demonstrates how unpatched, outdated services can lead to total system compromise.
