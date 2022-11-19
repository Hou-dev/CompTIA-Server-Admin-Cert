## CompTIA Server Administrator Certification

This repo will document my journey in getting the CompTIA server Administrator Certification and what resources I've studies in the hopes of helping other people in the future.

Some common information needed before proceeding:

1. What in the function of the rail system in a server? **Ans: Easy Maintenance**

2. How are servers measured? **Ans: U Form Factor**

3. What can RAID 1 be also called? **Ans: Mirroring**

4. What does PXE boot useful for? **Ans: Imaging and Remote Booting**

5. What are shares when talking about VMs? **Ans: Allocation of CPU resource**

6. How does a SAN communicate? **Ans: Fibre Channel**

7. Why implement a NAS? **Ans: Inexpensive**

8. What replaced BIOS on modern systems? **Ans: UEFI**

9. What does a DHCP server do? **Ans: Issues IP Configs.**

10. What are IOPS used to describe? **Ans: Disk Performance**

11. What resource should be increased as the number of printer users increase? **Ans: Memory**

12. Wevutil CLI used for? **Ans: Manages log files**

13. Number of drives required for RAID 5? **Ans: 3 Drives**

14. Host based firewall on Linux? **Ans: iptables**

15. What is CAT5 Ethernet max speed? **Ans: 100 Mbps**

16. What is a Zombie process? **Ans: Process that completes, but marked as dead as mistake.**

17. Port 443 used for? **Ans: HTTPS**

18. Another name for a Remote Access Trojan? **Ans: Backdoor**

19. Unique identifier for a MAC address vendor? **Ans: OUI**

20. How do you verify the integrity of a file? **Ans: Use Checksums**

21. How many tapes does a GFS system need? **Ans: 3**

22. IPSec used for? **Ans: Establishes a secure connection between two devices**

23. What does IPS useful for? **Ans: Monitor the network connections for Malicious activity.**

24. What is the "tracert" command used for on Windows? **Ans: Shows** the path taken to a destination network.

25. What device can be used for port security? **Ans: Switch**

26. How do you list disks on a Linux? **Ans: fdisk -l**

27. What is fstab used for on Linux? **Ans: Mount Partitions**


# Part 1

## Server Hardware

### Racking
Racking is the process of population a rack mounted into a rack system. These devices include routers, switches, ids, servers,etc.

### U Sizes
Each U is approximately 1.75 inches (4.45 cm) or 44.45 mm high. A rack can be 19 inches (ca. 48 cm) to 23 inches (0.58 m) in width.

### Thermal Dissipation
Removal of heat can be done with a Hot aisle and Cold aisle configuration. Which involves lining the racks into alternating rows of cold air intakes and hot air exhausts.

### Shrouds
Are used to direct airflow over components.

### Fans
Are used to assist a heat sink in removal of heat.

### Power Distribution Unit
PDUs can provide power conditioning, surge protection, case alarm and environment monitoring.

### KVM (Keyboard Video Mouse)
Allows management of multiple systems using single keyboard and mouse.

### Serial Connection
Allows for management of systems without being physically at the location.

### Voltage
The amount of Amps X Volts will give the Watts. Most power supplies can provide a range of voltages from 100-250V\

### Guidelines for U size servers.
1U (300-350W), 2U (350-400W), 4U(600-1000W) and Blade Servers(Depends on the number of blades, typically 4500W per chassis). Datacenters typically requires 2X the amount of power required by their servers.

### Total Power Draw
Sum the total amount of watts from the devices. Multiply the VA by 0.67 to get the power draw.

### Max load on a UPS
Mutiply VA by 0.8 to get the max load.

### Redundant PSUs
Most Data centers will have two PDUS connected to diffrent power grids to provde redundancy to their servers.

### Power Connector Types
Edison and Twist Lock

### Redundant Networking
The process of installing multiple network interface cards (NICs)

### STP and UTP
UTP offers no shielding around twisted pairs. STP has a foil around twisted pairs to protect from EMI.

### Patch Cables (Crossover and Straight Through)
Crossover cables are used to connect similar devices ex. Router to Router while Straight through connects dissimilar devices such as Server to a router.

### CAT5, RJ45 and RJ11
Categeory 5 cable transmitts 100 Mbps, RJ11 connector has 2 twisted pairs common on LAN lines while RJ45 connector 4 twisted pair common in ethernet cables.

### Fiber Connectors
SC (Subscriber connector) aka square connector. Uses a latch mechanism for release.
ST (Straight Tip) develop by AT&T and is the most widely used connector.
LC (Local Connector) popular in Fiber channel adapters, fast storage area networks or gigabit adapters.

### Single Mode vs MultiMode Fiber
Single mode connector uses a single beam of light for communication which allows for longer distances of travel. MultiMode uses many light beams through the cable.

### Gigabit vs 10 Gigabit
Gigabit usually maxes out on a CAT5e while 10 gigbit requires CAT6 which can only offer 100 meters at that speed.

### SFP Small Form-Factor Pluggable
SFP is a connector not standardized by th IEEE. SFP sockets are found in Ethernet switches, routers, firewalls, and network interface cards. SFP offers speed 1 gigabit to 4 Gbit/s while SFP+ offers 10-25 Gbit/s. QSFP offers 100 Gbit/s and 200 Gbit/s depending on the standard.

### Types of Server Chassis
1. Tower very similar to desktop towers. 
2. Rack Mount allows for fitment to stadard sized bays and require a rail kit. 
3. Blades thin modular circuit borads that can be easily slot in.

### CPU
Central processing Unit. Speed is measured in GHZ or MHZ. Typically fit a LGA or PGA sockets. They typically have three layers of cache. L1 smallest and closest the CPU, L2 larger and holds data exiting the CPU to the RAM. L3 is the largest and has to most latency. Typical architecture of CPUs are X86/x64 and ARM.

### RAM
ECC VS NON-ECC 
ECC offers error correcting properties. ECC is slower and more expensive. An algorithm is used when the ram is accessed and deemed vailed when the results are all Zeros. Non ECC is more common and can be found on consumer desktops and laptops.

### Interface Types
1. PCI standard on motherboard now replaced by PCI-E
2. PCI-X a double-wide version of the 32bit PCI local.
3. PCI-E uses a network of serial interconnects that operate at high speed.

