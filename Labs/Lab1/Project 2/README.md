# *Two Switches and Router (MultiSwitchNet-10)*

## *Project Overview*

*MultiSwitchNet-10* is an advanced topology featuring two switches and a router. It demonstrates inter-network communication by using both Class B (160.160.x.x) and Class C (192.168.0.x) IP addressing schemes.

## *Network Topology*

- **2 x Cisco 2960 Switches**
- **1 x Router**
- **5 x Devices per Switch**
- **Connections:** Each switch is connected to the router. Devices are connected to their respective switches using Copper Straight-Through cables.

## *IP Addressing Scheme*
### **Switch 1 (Class B Network)**

 - Network: 160.160.x.x
 - Subnet Mask: 255.255.0.0
 - IP Range: 160.160.1.1 - 160.160.1.5

### **Switch 2 (Class C Network)**

 - Network: 192.168.0.x
 - Subnet Mask: 255.255.255.0
 - IP Range: 192.168.0.1 - 192.168.0.5
  
```plaintext
Device     IP Address      Subnet Mask
--------------------------------------
PC1        160.160.1.1      255.255.0.0
PC2        160.160.1.2      255.255.0.0
PC3        160.160.1.3      255.255.0.0
PC4        160.160.1.4      255.255.0.0
PC5        160.160.1.5      255.255.0.0
...        ...            ...
Laptop1    192.168.0.1      255.255.255.0
Laptop2    192.168.0.2      255.255.255.0
Laptop3    192.168.0.3      255.255.255.0
Laptop4    192.168.0.4      255.255.255.0
Laptop5    192.168.0.5      255.255.255.0

```
