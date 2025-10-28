# Network_traffic_using_wireshark
# 🕵️‍♂️ Task 5 – Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
To capture live network packets using Wireshark and analyze common network protocols such as TCP, DNS, and HTTP.

---

## 🧰 Tools Used
- **Wireshark** – for packet capturing and analysis  
- **Kali Linux** – operating system used for performing the capture  
- **Firefox Browser / Ping utility** – for generating network traffic  

---

## ⚙️ Steps Performed
1. Installed Wireshark on Kali Linux using:
   ```bash
   sudo apt update
   sudo apt install wireshark -y
2.Selected the active Wi-Fi interface and started live packet capture.

3.Generated traffic by browsing multiple websites (e.g., google.com, youtube.com).

4.Captured packets for around one minute.

5.Stopped capture and saved results as Netwrok_traffic.pcapng.

6.Applied protocol filters in Wireshark:

tcp

dns

http

🌐 Protocols Identified
Protocol	Description	Example Observation
TCP (Transmission Control Protocol)	Ensures reliable communication between systems. Used by most web services.	Observed multiple TCP connections established during web browsing.
DNS (Domain Name System)	Resolves human-readable domain names into IP addresses.	DNS queries like www.google.com → 142.250.x.x.
HTTP (HyperText Transfer Protocol)	Used for transferring webpage data between client and server.	Observed HTTP requests/responses over TCP port 80.

🔍 Observations

DNS packets were seen resolving domain names before TCP connections were established.

TCP packets dominated the capture as they handle the main data exchange for browsing.

HTTP packets were visible as plaintext web traffic over port 80.

Some HTTPS (TLS-encrypted) traffic might appear as TCP due to encryption.

