# Task 5: Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
To capture live network packets using Wireshark, identify basic protocols, and analyze their purpose in network communication.

## 🛠 Tools Used
- **Kali Linux**
- **Wireshark**

## 📋 Steps Performed

1. **Launched Wireshark** in Kali Linux using:
   ```bash
   wireshark
## Steps Performed

- Selected the active network interface (`wlan0` for Wi-Fi in my case).
- Started packet capture and generated traffic by:
  - Visiting multiple websites.
  - Running ping commands:
    ```bash
    ping google.com
    ```
- Stopped capture after ~1 minute.
- Applied protocol filters in Wireshark:
  - `dns`
  - `arp`
  - `icmp`
- Noted down packet details for each protocol.
- Saved the capture as `task5.pcap`.
- Took screenshots of filtered packet views and details.

---

## 📊 Protocols Identified

| Protocol | Purpose | Example Packet Info |
|----------|---------|----------------------|
| **DNS**  | Resolves domain names to IP addresses | Query: `A google.com` |
| **ARP**  | Maps IP addresses to MAC addresses | Who has 192.168.0.1? Tell 192.168.0.10 |
| **ICMP** | Tests network connectivity | Echo request to 8.8.8.8 |

---

## 📂 Files in This Repository
- `task5.pcap` – Packet capture file.
- `README.md` – This documentation.
- `screenshots/` – Contains screenshots of Wireshark capture and analysis.

---

## 📸 Screenshots
- **DNS Packet Filter**
- **ARP Packet Filter**
- **ICMP Packet Filter**

---

## 🧠 Key Learnings
- Wireshark is a powerful tool for capturing and analyzing network traffic.
- Protocol filtering helps in quickly locating relevant packets.
- DNS, ARP, and ICMP each serve unique roles in network communication.
