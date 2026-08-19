# Subnetting

## What I Learned

**Subnetting** is the process of dividing one large network into smaller networks called **subnets**.

It helps organize networks, use IP addresses efficiently, and separate devices into different network segments.

---

## Simple Example

Suppose we have:

```text
192.168.1.0/24
```

A `/24` network has:

```text
256 total addresses
254 usable host addresses
```

We can divide it into smaller `/26` networks.

```text
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
```

So one `/24` network becomes **4 smaller `/26` networks**.

---

## Important Terms

### Network Address

The first address of a subnet.

Example:

```text
192.168.1.0
```

### Broadcast Address

The last address of a subnet, used to communicate with all devices in that subnet.

Example:

```text
192.168.1.63
```

### Usable Host Addresses

The addresses between the network and broadcast addresses.

For:

```text
192.168.1.0/26
```

Usable hosts are:

```text
192.168.1.1 - 192.168.1.62
```

---

## /26 Example

```text
Network:     192.168.1.0
First Host:  192.168.1.1
Last Host:   192.168.1.62
Broadcast:   192.168.1.63
```

Total addresses:

```text
64
```

Usable host addresses:

```text
62
```

---

## Why Subnetting Is Used

- Organize large networks
- Reduce unnecessary network traffic
- Separate groups of devices
- Use IP addresses efficiently
- Improve network management

---

## Subnet Mask vs Subnetting

**Subnet Mask:**

Defines the network and host portions of an IP address.

**Subnetting:**

Divides one network into smaller networks.

---

## Key Memory

> **Subnetting = dividing one big network into smaller networks.**

## What I Learned

- Subnetting divides a network into smaller subnets.
- `/24` can be divided into four `/26` networks.
- Every subnet has a network address and broadcast address.
- Usable host addresses are normally between the network and broadcast addresses.