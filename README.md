# Task 1: Scan Your Local Network for Open Ports Using Nmap

## 1. Objective
To discover devices connected to a local network, identify their open ports and understand possible network security risks using Nmap.

## 2. Tools Used
- Nmap
- Zenmap (Nmap GUI)
- Windows 10/11
- Command Prompt

## 3. Network Information

- Network Range: `192.168.1.0/24`
- Scanning Method: TCP SYN Scan
- Scan Command: `nmap -sS 192.168.1.106/24`

## 4. Procedure

1. Installed Nmap on the Windows system.
2. Opened Zenmap to perform network scanning.
3. Entered the local network range in the Target field.
4. Selected the TCP SYN scan command (`-sS`).
5. Started the scan to discover active devices.
6. Identified open, closed and filtered ports.
7. Studied the services running on open ports.
8. Analyzed possible security risks.

## 5. Scan Results

The scan discovered the following active devices:

| IP Address | Open Ports | Services |
|---|---|---|
| 192.168.1.1 | 22, 23, 53, 80, 1900 | SSH, Telnet, DNS, HTTP, UPnP |
| 192.168.1.102 | None detected | No open ports detected |
| 192.168.1.103 | None detected | Port 5060 filtered |
| 192.168.1.104 | None detected | No open ports detected |
| 192.168.1.105 | 135, 139, 445, 8081 | MSRPC, NetBIOS, Microsoft-DS, Blackice-icecap |
| 192.168.1.106 | Refer to complete scan output | Scan results partially visible |

## 6. Common Port Information

| Port | Service | Purpose |
|---|---|---|
| 22 | SSH | Secure remote login |
| 23 | Telnet | Remote login |
| 53 | DNS | Domain name resolution |
| 80 | HTTP | Web communication |
| 135 | MSRPC | Windows remote procedure calls |
| 139 | NetBIOS | Network communication |
| 445 | SMB | File and printer sharing |
| 1900 | UPnP | Device discovery |
| 8081 | HTTP alternative | Web service |

## 7. Security Risks Identified

1. Telnet (Port 23) may transmit login information without encryption.
2. SSH (Port 22) should use strong authentication.
3. HTTP (Port 80) does not encrypt communication by itself.
4. SMB (Port 445) may expose shared resources if improperly configured.
5. UPnP (Port 1900) may expose devices to unwanted network access.
6. Unnecessary open ports should be disabled or restricted.

## 8. Learning Outcomes

- Learned basic network reconnaissance.
- Understood how to use Nmap and Zenmap.
- Identified active devices on a local network.
- Learned about open, closed and filtered ports.
- Understood common network services and their security risks.
- Gained practical knowledge of network exposure.

## 9. Conclusion

Successfully performed a local network scan using Nmap and Zenmap. Identified active devices, discovered open ports and studied the services running on them. This practical helped me understand basic network reconnaissance and network security.

## 10. Screenshots

The screenshots of the Nmap scanning process and results are included in this repository.
