# Subnetting Cheatsheet

## 📘 Key Concepts
- **IP Address**: A 32-bit number divided into 4 octets (e.g., 192.168.1.10).
- **Subnet Mask**: Defines the network and host portion of the IP address.
- **CIDR Notation**: Shorthand for subnet masks (e.g., /24 = 255.255.255.0).
- **Network Address**: First address in the subnet (all host bits = 0).
- **Broadcast Address**: Last address in the subnet (all host bits = 1).
- **Usable Hosts**: Number of valid devices that can be assigned in the subnet.

---

## 🧮 Subnetting Formulas
- **Number of Subnets** = 2^borrowed_bits  
- **Number of Hosts per Subnet** = 2^host_bits – 2  
  (subtract 2 for network + broadcast addresses)

---

## 📊 Quick Reference Table

| CIDR | Subnet Mask      | # of Subnets | # of Hosts/Subnet |
|------|------------------|--------------|-------------------|
| /24  | 255.255.255.0    | 1            | 254               |
| /25  | 255.255.255.128  | 2            | 126               |
| /26  | 255.255.255.192  | 4            | 62                |
| /27  | 255.255.255.224  | 8            | 30                |
| /28  | 255.255.255.240  | 16           | 14                |
| /29  | 255.255.255.248  | 32           | 6                 |
| /30  | 255.255.255.252  | 64           | 2                 |

---

## 📝 Example Problem
**Q:** You are given `192.168.10.0/26`.  
- What is the subnet mask?  
- How many subnets?  
- How many usable hosts?  
- First valid host? Last valid host?

**Solution:**
- Subnet mask = 255.255.255.192  
- # of subnets = 4 (because 2^2 borrowed bits = 4)  
- # of usable hosts = 62 (2^6 – 2 = 62)  
- Subnets are broken into blocks of 64:  
  - 192.168.10.0 → Network  
  - 192.168.10.1 → First host  
  - 192.168.10.62 → Last host
