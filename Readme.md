# Basic Network Scanning with Nmap

*Objective*

To perform a network scan on the local machine using Nmap and identify open ports and services.

*Tool Used*

- Nmap 7.99

*Commands Executed*

```bash
nmap --version
nmap localhost
nmap -sV localhost
```

*Results*

The scan identified the following open ports and services:

| Port | State | Service | Version |
|------|--------|---------|---------|
| 135/tcp | Open | msrpc | Microsoft Windows RPC |
| 445/tcp | Open | microsoft-ds | SMB File Sharing |

*Significance of Open Ports*

*Port 135 (MSRPC)*

Microsoft Remote Procedure Call (RPC) allows communication between Windows applications and services. It is commonly used for administrative tasks and remote management.

*Port 445 (Microsoft-DS)*

Port 445 is used by the Server Message Block (SMB) protocol for file and printer sharing across Windows networks.

*Conclusion*

Nmap successfully scanned the local machine and identified active services running on open ports. Understanding open ports helps administrators detect potential security risks and manage network services effectively.