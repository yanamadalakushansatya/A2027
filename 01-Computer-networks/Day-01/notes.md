
# Day 01 — Networking Fundamentals

## Environment
- OS: Fedora Linux
- Network interface: wlp2s0
- IPv4: 192.168.0.107/24
- Default gateway: 192.168.0.1

## Commands Practiced

### 1. Network Interfaces
`ip -br addr`

Identified the loopback and Wi-Fi interfaces.

### 2. Routing Table
`ip route`

Identified the default gateway and local network route.

### 3. Gateway Connectivity
`ping -c 4 192.168.0.1`

Result: 4 transmitted, 4 received, 0% packet loss.

### 4. Internet Connectivity
`ping -c 4 8.8.8.8`

Result: 4 transmitted, 4 received, 0% packet loss.

### 5. DNS Connectivity
`ping -c 4 google.com`

Result: 4 transmitted, 4 received, 0% packet loss.

### 6. DNS Configuration
`resolvectl status`

Inspected configured DNS servers.

### 7. DNS Resolution
`resolvectl query google.com`

Successfully resolved IPv4 and IPv6 addresses.

## Key Learnings
- Loopback works without internet connectivity.
- A default gateway forwards traffic toward external networks.
- An operational Wi-Fi interface does not guarantee internet access.
- DNS resolves domain names into IP addresses.
- Multiple DNS servers can provide redundancy.
