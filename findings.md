# Wireshark Network Traffic Analysis

## Objective

The objective of this project is to capture and analyse network traffic using Wireshark.

---

## 1. DNS Analysis

Filter Used:

dns

Screenshot:

<img width="958" height="434" alt="dns-analysis" src="https://github.com/user-attachments/assets/4c98b6f5-e750-44e1-bcb9-30a9b2f52f6e" />

Observation:

* A DNS query was captured for github.com.
* The client system sent a request to the local DNS server.
* DNS uses UDP port 53 for domain name resolution.
* DNS translates domain names into IP addresses before communication can begin.

---

## 2. HTTPS/TLS Analysis

Filter Used:

tls

Screenshot:

<img width="1857" height="1093" alt="image" src="https://github.com/user-attachments/assets/b065a380-32b5-48d5-988e-ab3d92642897" />


Observation:

* TLSv1.3 traffic was observed between the client and a remote server.
* A Client Hello and Server Hello exchange was captured.
* Communication occurred over TCP port 443.
* HTTPS encrypts data to protect confidentiality and integrity during transmission.

---

## 3. TCP Handshake Analysis

Filter Used:

tcp

Screenshot:

<img width="959" height="437" alt="Screenshot 2026-06-23 105200" src="https://github.com/user-attachments/assets/6e06b97e-c6af-453e-a738-374159512d29" />

Observation:

* A TCP three-way handshake was captured.
* The client initiated the connection by sending a SYN packet.
* The server responded with a SYN-ACK packet.
* The client completed the connection establishment by sending an ACK packet.
* This process is used to establish reliable communication before data transmission begins.

---

## 4. ICMP Analysis

Filter Used:

icmp

Screenshot:

<img width="959" height="431" alt="Screenshot 2026-06-23 105848" src="https://github.com/user-attachments/assets/fd37c847-987d-4684-9701-544315351336" />

Observation:

* ICMP echo request and echo reply packets were captured.
* The ping command was used to test connectivity between the client and a remote host.
* Successful replies confirmed that the destination host was reachable.
* ICMP is commonly used for network troubleshooting and connectivity testing.

---

## Conclusion

This project demonstrated basic network traffic analysis using Wireshark. DNS queries, TCP connection establishment, HTTPS/TLS communication and ICMP traffic were successfully captured and analysed. These protocols are commonly encountered during cybersecurity investigations and network monitoring activities.
