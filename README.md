# CCNA Networking Basics - Packet Tracer Labs

Welcome to the **CCNA Networking Basics Packet Tracer Labs** repository! This collection of labs is designed to help beginners understand fundamental networking concepts, focusing on router configuration and security.

## 🚀 Overview
These labs are intended to provide hands-on practice using Cisco Packet Tracer. Each lab includes step-by-step instructions, configuration commands, and explanations to reinforce key networking concepts.

## 📌 Topics Covered
- **Basic Router Configuration**
- **IP Addressing & Subnetting**
- **Static & Dynamic Routing (RIP, OSPF, EIGRP)**
- **VLANs & Inter-VLAN Routing**
- **Access Control Lists (ACLs)**
- **Network Address Translation (NAT)**
- **DHCP & DNS Configuration**
- **SSH & Password Security**
- **Firewall & Security Best Practices**

## 🏗️ Lab Structure
Each lab is structured as follows:
1. **Objective** - A brief explanation of what you will learn.
2. **Topology** - A visual representation of the network.
3. **Commands & Configuration** - Step-by-step CLI commands.
4. **Verification & Testing** - How to test your setup.
5. **Troubleshooting Tips** - Common issues and solutions.

## 📖 Sample Router Configuration
Here’s a basic router configuration setup:

```bash
# Enter privileged EXEC mode
enable

# Configure a hostname
configure terminal
hostname Router1

# Set a secure enable password
enable secret StrongPassword

# Configure IP address for an interface
interface GigabitEthernet0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit

# Configure SSH for secure remote access
ip domain-name example.com
crypto key generate rsa modulus 1024
username admin secret AdminPass
line vty 0 4
login local
transport input ssh
exit

# Save configuration
write memory
```

## 📂 How to Use
1. Clone the repository:
   ```sh
   git clone https://github.com/benir-0/ccna-networking.git
   ```
2. Open the `.pkt` files in **Cisco Packet Tracer**.
3. Follow the instructions in each lab folder.
4. Experiment with different configurations!

## 📢 Contributions
Feel free to contribute additional labs, improvements, or fixes! Just fork the repo and submit a pull request.


## 📧 Contact
For questions or suggestions, reach out via [beniromenda@gmail.com] or open an issue in the repository.

Happy networking! 🌐

