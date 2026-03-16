## Subnetting Basics

### What is Subnetting
Subnetting = the process of dividing a network into smaller networks (subnets).

Purpose:
- better network organization
- improved security
- more efficient traffic management

Example:
A company might split the network into departments:
- Accounting
- Human Resources
- Finance

Each department can have its own subnet.

---

### IP Address Structure

An IPv4 address has **32 bits** divided into **4 octets**.

Example:

192.168.1.1

Octets range from:

0 - 255

---

### Subnet Mask

A subnet mask determines which part of an IP address belongs to:

- the **network**
- the **host**

Example:

IP Address  
192.168.1.100

Network Address  
192.168.1.0

---

### Types of Addresses

#### Network Address
Identifies the **network itself**

Example:

192.168.1.0

---

#### Host Address
Identifies a **device inside the network**

Example:

192.168.1.100

---

#### Default Gateway
The device that sends traffic **outside the network**.

Usually the **router**.

Typical addresses:

192.168.1.1  
or  
192.168.1.254

---

### Why Subnetting Matters

Benefits:
- Efficiency
- Security
- Network control

Example:

A café network may separate:

- staff network
- public WiFi

This prevents public users from accessing internal systems.
