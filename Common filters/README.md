# 🔍 Common Wireshark Filters

| **Filter** | **Purpose** |
|------------|-------------|
| `arp` | Show ARP packets |
| `dns` | Show DNS traffic |
| `tcp` | Show TCP packets |
| `udp` | Show UDP packets |
| `icmp` | Show Ping (ICMP) packets |
| `http` | Show HTTP traffic |
| `tls` | Show HTTPS/TLS traffic |
| `dhcp` | Show DHCP packets |

## 🌐 IP Filters

```text
ip.addr == 192.168.1.10
```
Shows packets to/from a specific IP.

```text
ip.src == 192.168.1.10
```
Shows packets from a specific IP.

```text
ip.dst == 192.168.1.10
```
Shows packets to a specific IP.

## 🚩 TCP Flag Filters

```text
tcp.flags.syn == 1
```
Shows SYN packets.

```text
tcp.flags.syn == 1 && tcp.flags.ack == 1
```
Shows SYN-ACK packets.

```text
tcp.flags.fin == 1
```
Shows FIN packets.

## 🔌 Port Filters

```text
tcp.port == 80
```
HTTP traffic.

```text
tcp.port == 443
```
HTTPS traffic.

```text
tcp.port == 22
```
SSH traffic.
