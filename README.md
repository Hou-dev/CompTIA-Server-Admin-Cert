
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

The amount of Amps X Volts will give the Watts. Most power supplies can provide a range of voltages from 100-250V

  

### Guidelines for U size servers.

1U (300-350W), 2U (350-400W), 4U(600-1000W) and Blade Servers(Depends on the number of blades, typically 4500W per chassis). Datacenters typically requires 2X the amount of power required by their servers.

  

### Total Power Draw

Sum the total amount of watts from the devices. Multiply the VA by 0.67 to get the power draw.