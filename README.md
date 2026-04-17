# wireshark-network-analysis
Task 5 - Network Traffic Analysis using Wireshark

Network Traffic Analysis باستخدام Wireshark

Task 5: Capture and Analyze Network Traffic Using Wireshark

---

Objective

The objective of this task is to capture live network traffic and analyze it to identify common protocols and traffic types. This helps in understanding how data flows across a network and builds practical packet analysis skills.

---

Tools Used

* Wireshark (Network Protocol Analyzer)
* Web Browser (for generating traffic)
* Command Prompt (for ping command)
* Operating System: Windows 10/11

---

Procedure

1. Install Wireshark

Downloaded and installed Wireshark from the official website.

 2. Start Packet Capture

* Open Wireshark
* Select active network interface (Wi-Fi/Ethernet)
* Click on **Start Capture**

3. Generate Network Traffic

Performed the following actions to generate traffic:

* Opened websites in browser
* Executed command:

```bash
ping google.com
```

4. Stop Packet Capture

* Captured packets for about 1 minute
* Clicked on **Stop Capture**

5. Apply Filters

Used the following filters to analyze specific traffic:

```
dns
tcp
icmp
```
6. Export Capture File



7. Protocols Identified

1. DNS (Domain Name System)

* Resolves domain names to IP addresses
* Observed when accessing websites

**Example:**

* Query for `google.com`

---

2. TCP (Transmission Control Protocol)

* Ensures reliable communication
* Observed TCP 3-way handshake:

  * SYN
  * SYN-ACK
  * ACK


3. ICMP (Internet Control Message Protocol)

* Used for network diagnostics
* Observed during ping command:

  * Echo Request
  * Echo Reply

Sample Analysis

| Protocol | Description            | Example Activity     |
| -------- | ---------------------- | -------------------- |
| DNS      | Resolves domain names  | Accessing google.com |
| TCP      | Reliable communication | Opening websites     |
| ICMP     | Connectivity testing   | ping google.com      |

Findings

* DNS traffic was observed when resolving domain names
* TCP packets established communication between client and server
* ICMP packets confirmed connectivity using ping

These protocols work together to enable normal internet communication.

Outcome

* Successfully captured live network traffic
* Identified key protocols: DNS, TCP, ICMP
* Learned packet filtering and analysis
* Exported capture file in `.pcap` format

Conclusion

This task provided hands-on experience with network packet analysis using Wireshark and improved understanding of how different protocols interact in real-time communication.
