# 🌐 OSI Model (Open Systems Interconnections)
The OSI model is a framework that explains how two devices communicate with each other and how data is travelled from one device to another through network in 7 layers. Each layer communicate with layer above or below it and every layer has its own specific job.

---

## ☰ The 7 layers

| Layer | Name                | What It Does                                      | Example                 |
|-------|---------------------|---------------------------------------------------|-------------------------|
| 7     | Application         | User interface and software (apps)                | Web browser, Email app  |
| 6     | Presentation        | Data formatting and encryption                    | JPEG, SSL/TLS           |
| 5     | Session             | Manages connections and sessions                  | API sessions, logins    |
| 4     | Transport           | Delivers data reliably (or fast)                  | TCP, UDP                |
| 3     | Network             | Finds the best route for data                     | IP Addressing, Routers  |
| 2     | Data Link           | Handles frames and MAC addresses                  | Switches, Ethernet      |
| 1     | Physical            | Sends bits over wires or Wi-Fi                    | Cables, Wi-Fi, NIC      |

---

## 🔄 Real-Life Example (Visiting a Website)

1. **Application (Layer 7):** You type a URL in your browser.
2. **Presentation (Layer 6):** Data is encrypted with HTTPS (SSL).
3. **Session (Layer 5):** A session is made between your browser and the server.
4. **Transport (Layer 4):** TCP breaks the data into packets.
5. **Network (Layer 3):** The IP address helps route the data.
6. **Data Link (Layer 2):** Your router uses MAC address to send frames.
7. **Physical (Layer 1):** Data travels through cables or Wi-Fi as bits.

---

## 🔐 Why It's Important in Cybersecurity

- Helps identify which layer an attack targets (e.g., DDoS = Layer 3/4)
- Useful when analyzing packet captures with tools like Wireshark
- Makes troubleshooting easier during CTFs or lab exercises

---

💬 So this was all about OSI model, make sure to see other notes on networking in this folder.
