# 🛡️ **Nmap Command Reference Guide**  
Unlock the full potential of Nmap with this detailed reference for network scanning, service discovery, and security auditing.

![Network Security](https://img.shields.io/badge/Network%20Security-Tools-green)

---

## 📋 **Contents**
1. [Introduction to Nmap](#introduction-to-nmap)
2. [Basic Scanning Techniques](#basic-scanning-techniques)
3. [Port Scanning and Analysis](#port-scanning-and-analysis)
4. [Service Discovery & Version Detection](#service-discovery--version-detection)
5. [Advanced Scanning Techniques](#advanced-scanning-techniques)
6. [Scripting & Automation](#scripting--automation)
7. [Output & Reporting](#output--reporting)
8. [Performance & Timing Adjustments](#performance--timing-adjustments)
9. [Firewall Evasion Techniques](#firewall-evasion-techniques)
10. [Extra Features & Options](#extra-features--options)

---

## 📖 **Introduction to Nmap**
Nmap (Network Mapper) is an open-source tool for network exploration and security auditing. It allows network administrators and security professionals to discover devices and services on a network, and identify vulnerabilities. 

---

## 📐 **Basic Scanning Techniques**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap <target ip>`              | Scan a single host or device                 |
| `nmap <target1 target2>`        | Scan multiple hosts or devices               |
| `nmap -iL targets.txt`          | Scan targets from a file                     |
| `nmap -sn <target>`             | Host discovery (ping scan)                   |

---

## 🛠️ **Port Scanning and Analysis**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -p <port> <target>`       | Scan a specific port                         |
| `nmap -p- <target>`             | Scan all 65,535 ports                        |
| `nmap -F <target>`              | Scan the 100 most common ports               |
| `nmap -p 20-100 <target>`       | Scan a range of ports                        |

---

## 🔍 **Service Discovery & Version Detection**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -sV <target>`             | Detect services and their versions           |
| `nmap -A <target>`              | Aggressive scan (includes OS detection)      |
| `nmap --version-intensity 0-9 <target>` | Adjust version detection depth             |

---

## ⚡ **Advanced Scanning Techniques**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -sS <target>`             | SYN scan (stealth scan)                      |
| `nmap -sT <target>`             | Connect scan (TCP)                           |
| `nmap -sU <target>`             | UDP scan                                     |
| `nmap -sA <target>`             | ACK scan                                     |
| `nmap -sN <target>`             | NULL scan (no flag set)                      |
| `nmap -sF <target>`             | FIN scan (FIN flag set)                      |
| `nmap -sX <target>`             | XMAS scan (FIN, URG, and PSH flags set)      |
| `nmap -sO <target>`             | Protocol scan (Determine supported protocols) |
| `nmap -sP <target>`             | Ping scan (no port scan)                     |

---

## 📜 **Scripting & Automation**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap --script <scriptname> <target>` | Run a specific Nmap script                 |
| `nmap --script vuln <target>`   | Scan for vulnerabilities using scripts       |
| `nmap --script-help <scriptname>` | Get help for a specific script             |

---

## 📑 **Output & Reporting**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -oN output.txt <target>`  | Save scan results in a normal output file    |
| `nmap -oX output.xml <target>`  | Save scan results in XML format              |
| `nmap -oG output.grep <target>` | Save scan results in grepable format         |

---

## ⏱️ **Performance & Timing Adjustments**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -T<0-5> <target>`         | Set the scan timing (0=paranoid, 5=fastest)   |
| `nmap --max-retries 3 <target>` | Limit the number of retries                  |
| `nmap --max-scan-delay <time> <target>` | Adjust delay between probe attempts      |

---

## 🛡️ **Firewall Evasion Techniques**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -f <target>`              | Use fragmented IP packets                    |
| `nmap --mtu <value> <target>`   | Set Maximum Transmission Unit (MTU) for evasion |
| `nmap --data-length <value> <target>` | Add random data to packets                |

---

## 🔧 **Extra Features & Options**
| **Command**                     | **Description**                              |
|---------------------------------|----------------------------------------------|
| `nmap -v <target>`              | Increase verbosity (use multiple times for more details) |
| `nmap -d <target>`              | Display debug output                         |
| `nmap --stats-every <time> <target>` | Show periodic stats while scanning         |

---

## 📂 **Examples of Nmap Commands**
- **Scan a single target**:  
  ```bash
  nmap 192.168.1.1
  ```
- **Scan multiple targets**:

  ```bash

  nmap 192.168.1.1 192.168.1.2
  ```
- **Scan a range of ports**:

  ```bash
  
  nmap -p 20-100 192.168.1.1
  ```
  - **Run an aggressive scan with OS detection**:
  
  ```bash
 
  nmap -A 192.168.1.1
  ```
  - **Save output in XML format**:
  
  ```bash
  nmap -oX output.xml 192.168.1.1
  ```
## 📚 Resources for Further Learning
- [Official Nmap Documentation](https://nmap.org/book/)
- [Nmap Scripting Engine Overview](https://nmap.org/book/nse.html)
- [Nmap Cheat Sheet by Offensive Security](https://www.offensive-security.com/nmap-cheat-sheet/)


```markdown


### Changes made:
1. **Improved Section Titles**: Headings like "Scan Types" have been refined to "Advanced Scanning Techniques" and others reworded for clarity.
2. **Enhanced Layout**: More consistent use of emojis to visually enhance different sections.
3. **Rephrased Descriptions**: Some command descriptions were rephrased to make the guide more user-friendly and professional.
4. **Clarified Examples**: Added a few more practical examples of how commands work.
```
