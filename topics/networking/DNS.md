# 🌍 Domain Name System (DNS)

The **Domain Name System (DNS)** eliminates the need to remember numerical IP addresses.  
It translates **domain names** (like `example.com`) into their corresponding **IP addresses** (like `93.184.216.34`).

In simple terms, DNS acts as the **“phone book of the internet.”**

---

## 🧩 Layer and Protocol

- **OSI Layer:** Application Layer (Layer 7)  
- **Transport Protocols:**  
  - **UDP Port 53** – Default and faster for most queries.  
  - **TCP Port 53** – Used for zone transfers or when UDP responses are too large.

---

## 🗂️ Common DNS Record Types

| Record | Name | Description |
|--------|------|--------------|
| **A** | Address | Maps a **hostname** to an **IPv4 address**. |
| **AAAA** | IPv6 Address | Maps a **hostname** to an **IPv6 address**. |
| **CNAME** | Canonical Name | Maps one **domain name** to another (alias). |
| **MX** | Mail Exchange | Specifies the **mail server** that handles emails for the domain. |

---

## ⚙️ DNS Lookup Example

You can query DNS information using the **`nslookup`** tool (available on Windows, macOS, and Linux):

```bash
nslookup example.com

Name:    example.com
Address: 93.184.216.34

```
## Summary
- DNS converts human-readable names into machine-readable IPs.

- Operates at Layer 7 of the OSI model.

- Uses port 53 for communication (UDP by default, TCP for fallback).

- Common record types include A, AAAA, CNAME, and MX.