# Kali Linux Setup on VirtualBox

## Project Overview
This project documents the configuration of Kali Linux as a cybersecurity testing machine using Oracle VirtualBox.

## Objectives
- Configure Kali Linux as an attacking and security testing machine.
- Configure a NAT Network using the `10.0.0.0/24` subnet.
- Assign Kali Linux the IP address `10.0.0.2/24`.
- Enable full internet access.
- Enable bidirectional clipboard and drag-and-drop.
- Configure a shared folder between the host and Kali Linux.

## Configuration Details

| Component | Required Configuration |
|---|---|
| Virtualization | Oracle VirtualBox |
| Operating System | Kali Linux |
| Network Mode | NAT Network |
| Subnet | `10.0.0.0/24` |
| Kali IP Address | `10.0.0.2/24` |
| Internet Access | Enabled |
| Shared Clipboard | Bidirectional |
| Drag and Drop | Bidirectional |
| Shared Folder | Host Downloads folder |

## Screenshots

### 1. VirtualBox Network Configuration
![VirtualBox Network](screenshots/virtualbox-network.png)

### 2. Kali Linux IP Address
![Kali IP Address](screenshots/kali-ip-address.png)

### 3. Internet Connectivity Test
![Internet Connectivity](screenshots/internet-connectivity.png)

### 4. Shared Folder Configuration
![Shared Folder](screenshots/shared-folder.png)

## Verification Commands

Check the IP address:
```bash
ip -br addr
```

Check the routing table:
```bash
ip route
```

Test internet connectivity:
```bash
ping -c 4 8.8.8.8
```

Test DNS resolution:
```bash
ping -c 4 google.com
```

## Learning Outcomes
- Learned to configure Kali Linux in VirtualBox.
- Practiced virtual network configuration.
- Verified IP addressing and internet connectivity.
- Configured host-to-guest file sharing.

## Disclaimer
This environment is intended for authorized cybersecurity learning and testing only.
