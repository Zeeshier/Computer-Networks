# *Router Between Network A and Network B*

## *Project Overview*

This Task demonstrates inter-network communication between two separate networks, Network A and Network B, using a router and multiple switches. The configuration showcases routing between a Class A network (50.0.0.x) and a Class B network (140.130.0.x) with proper gateway settings.
## *Network Topology*

- **1 x Router (Handles routing between Network A and Network B)**
- **4 x Cisco 2960 Switches**
  - 2 Switches in Network A
  - 2 Switches in Network B
- **20 x End Devices**
  - 10 PCs in Network A (5 per switch)
  - 10 Laptops in Network B (5 per switch)
- **Connections:**
  - Each switch is connected to the router via Copper Straight-Through cables.
  - Devices are connected to their respective switches using Copper Straight-Through cables.

## *IP Addressing Scheme*
### **Network A (Class A Network):** 
- **Network:** 50.0.0.x
- **Subnet Mask:** 255.0.0.0
- **IP Range:** 50.0.0.1 - 50.0.0.10
- **Gateway:** 50.0.0.11

### **Network B (Class B Network):** 
- **Network:** 140.130.0.x
- **Subnet Mask:** 255.255.0.0
- **IP Range:** 140.130.0.1 - 140.130.0.10
- **Gateway:** 140.130.0.11

## **Router Configuration**

The following commands configure the router to enable communication between Network A and Network B:
```plaintext
Router> enable
Router# configure terminal

# Configuring Interface for Network A
Router(config)# interface gig0/1
Router(config-if)# ip address 50.0.0.11 255.0.0.0
Router(config-if)# no shutdown

# Configuring Interface for Network B
Router(config)# interface gig0/1
Router(config-if)# ip address 140.130.0.11 255.255.0.0
Router(config-if)# no shutdown
```

  - **Author:** Zeeshan Ahmad
  - **Project:** Multi-Network Router Configuration

