# OSI Model

The OSI (Open Systems Interconnection) model is a conceptual framework developed by ISO (International Organization for Standardization) that describes how data is transmitted and received over a network.

In simple terms, it defines how computers communicate across networks by breaking communication into seven layers, each with a specific function.

# 🧩 OSI Model Layers
##	Layer	Description
1.	Physical Layer	Deals with the physical connection between devices (e.g., cables, connectors, wireless signals). Responsible for transmitting raw bits over a physical medium.

2.	Data Link Layer	Defines how data is transferred between nodes on the same network. Handles framing, addressing (MAC), and error detection.

3.	Network Layer	Handles communication between different networks. Manages logical addressing (IP addresses) and routing to deliver packets across networks.

4.	Transport Layer	Enables end-to-end communication, providing flow control, segmentation, and error correction. Common protocols: TCP and UDP.

5.	Session Layer	Manages sessions between applications — establishing, maintaining, and terminating connections. Common examples include NFS or RPC.

6.	Presentation Layer	Ensures data is in a usable format for the application. Handles encryption, compression, and encoding.

7.	Application Layer	Provides network services directly to end-user applications. Example: web browsers use HTTP to request web pages.

## Summary

The OSI model defines a standardized way for network communication.

Each layer depends on the layer below it and supports the layer above it.

Understanding the OSI model helps troubleshoot network issues and understand how protocols interact.

### 🧭 Quick Tip

Remember this mnemonic to recall the OSI layers (top to bottom):

"All People Seem To Need Data Processing"
→ Application → Presentation → Session → Transport → Network → Data Link → Physical