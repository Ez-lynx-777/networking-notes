## What I Learned

- ARP stands for Address Resolution Protocol.
- ARP is used to find the MAC address of a device when its IP address is known.
- ARP is mainly used on a local network.
- An ARP Request asks: "Who has this IP address?"
- The device with that IP sends an ARP Reply containing its MAC address.
- The IP-to-MAC mapping can be stored in the ARP cache.
- I can view my ARP cache using `arp -a`.
- ARP is important because devices use MAC addresses for local Ethernet communication.
- ARP spoofing/poisoning can abuse ARP by sending false IP-to-MAC mappings.

### Easy Memory

> **ARP = IP → MAC**

### Practical Command

```powershell
arp -a