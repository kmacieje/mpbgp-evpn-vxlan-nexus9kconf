# Thesis: Analysis and Evaluation of Overlay Networks in Data Centers

## Overview
This thesis analyzes and evaluates the performance of overlay networks by comparing two network architectures commonly used in data centers:
- **Traditional network architecture**
- **Modern Spine-Leaf architecture**

## Objectives
- Assess the theoretical requirements for modern data center networks.
- Identify limitations of outdated network solutions.
- Compare technologies and configurations used in both traditional and modern network designs.

## Key Findings
### Traditional Network Architecture
- **Technologies Used**:
  - Spanning Tree Protocol (STP) and its enhanced version, Rapid STP (RSTP), to prevent network loops.
  - VLANs for network segmentation.
  - Virtual interfaces on Layer 3 switches for inter-domain routing.
- **Limitations**:
  - Scalability challenges due to limited VLAN namespace.
  - Inefficient failure recovery mechanisms.

### Modern Spine-Leaf Architecture
- **Technologies Used**:
  - **VXLAN Overlay**: Extends the VLAN namespace, supporting larger-scale network segmentation.
  - Configuration divided into two layers:
    - **Underlay**: Ensures communication between VTEPs (VXLAN Tunnel Endpoints).
    - **Overlay**: Enables virtual network creation over physical infrastructure.
  - **MP-BGP with EVPN**: Manages BUM (Broadcast, Unknown unicast, Multicast) traffic efficiently.
- **Advantages**:
  - Improved scalability and flexibility.
  - Faster failure recovery and better support for high-speed transmission.

## Testing and Results
A series of tests were conducted to evaluate both architectures in terms of:
1. **Throughput** in both directions.
2. **Transmission efficiency** under varying data loads.
3. **Resilience to failures** and recovery speed.

**Key Results**:
- Modern Spine-Leaf architecture demonstrated:
  - High throughput under significant data loads.
  - Minimal packet loss at higher transmission speeds.
  - Rapid network recovery after failures.

## Future Prospects
- **Advancement of MP-BGP EVPN VXLAN**:
  - Potential for standardization and synchronization with cloud solutions.
  - Enhanced support for AI-driven networking solutions.

---

This thesis highlights the clear advantages of modern overlay network designs in data centers, paving the way for more scalable, efficient, and future-ready network architectures.
