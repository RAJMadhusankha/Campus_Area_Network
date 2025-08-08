# Campus Area Network - Cisco Packet Tracer Project

## 📋 Project Overview

This repository contains a comprehensive campus area network (CAN) design implemented using Cisco Packet Tracer. The project demonstrates enterprise-level network architecture with hierarchical design principles, VLAN segmentation, and multi-building connectivity.

## 🏗️ Network Architecture

### Topology Design
- **Type**: Campus Area Network (CAN)
- **Design Model**: Three-tier hierarchical (Core, Distribution, Access)
- **Coverage**: Multi-building campus environment
- **Connectivity**: Fiber backbone with Ethernet access

### Key Features
- ✅ Hierarchical network design
- ✅ VLAN segmentation for security and performance
- ✅ Redundant connectivity paths
- ✅ Inter-building fiber connectivity
- ✅ Scalable architecture
- ✅ Enterprise-grade equipment simulation

## 🌐 Network Components

### Infrastructure Equipment
| Device Type | Model | Quantity | Purpose |
|-------------|-------|----------|---------|
| Core Switch | Cisco 3560 | 2+ | High-speed core switching |
| Access Switch | Cisco 2960 | 10+ | End-device connectivity |
| Router | Various | 3+ | Inter-VLAN routing |
| Fiber Links | - | Multiple | Building interconnection |

### Network Segments
- **Building A**: Administrative and faculty network
- **Main Building**: Core infrastructure and servers  
- **Building B**: Student and general access network
- **Server Farm**: Centralized services and applications

## 🔧 Configuration Details

### VLAN Structure
```
VLAN 10 - Administration (192.168.1.x)
VLAN 20 - Faculty (192.168.2.x)
VLAN 30 - Students (192.168.3.x)
VLAN 40 - Servers (192.168.4.x)
VLAN 99 - Management (192.168.99.x)
```

### IP Addressing Scheme
- **Subnet Mask**: /24 (255.255.255.0)
- **Default Gateway**: .1 on each subnet
- **DHCP Range**: .10-.200 on each subnet
- **Static Range**: .201-.254 for servers/infrastructure


## 🚀 Getting Started

### Prerequisites
- Cisco Packet Tracer 8.0 or later
- Basic knowledge of networking concepts
- Understanding of Cisco IOS commands

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/campus-network.git
   cd campus-network
   ```

2. Open the `.pkt` file in Cisco Packet Tracer:
   ```
   File → Open → Campus_Area_Network.pkt
   ```

3. Start the simulation to test connectivity

### Quick Test Commands
```cisco
# Test connectivity
ping 192.168.1.1
ping 192.168.2.1

# View VLAN information
show vlan brief

# Check interface status
show ip interface brief

# View routing table
show ip route
```

## 📊 Network Testing

### Connectivity Tests
- [ ] Inter-VLAN communication
- [ ] Building-to-building connectivity
- [ ] Server accessibility from all VLANs
- [ ] Redundant path functionality
- [ ] DHCP assignment verification

### Performance Metrics
- **Convergence Time**: < 30 seconds
- **Ping Latency**: < 10ms within building
- **Throughput**: 100Mbps access, 1Gbps backbone
- **Packet Loss**: < 0.1%

## 🛠️ Customization

### Adding New Buildings
1. Add new switches to the topology
2. Configure VLANs for the new building
3. Update routing tables
4. Configure trunk links to core

### VLAN Modifications
1. Create new VLAN: `vlan [number]`
2. Assign name: `name [vlan-name]`
3. Configure access ports: `switchport access vlan [number]`
4. Update routing if needed

## 🔍 Troubleshooting

### Common Issues
| Issue | Symptoms | Solution |
|-------|----------|----------|
| No connectivity between VLANs | Can't ping other subnets | Check inter-VLAN routing |
| DHCP not working | No IP assignment | Verify DHCP pool configuration |
| Trunk not working | VLANs not passing | Check trunk configuration |

### Debug Commands
```cisco
show spanning-tree
show cdp neighbors
show mac address-table
debug ip routing
```

## 📈 Future Enhancements

### Planned Features
- [ ] Wireless network integration
- [ ] Network security implementation (ACLs)
- [ ] Quality of Service (QoS) configuration
- [ ] Network monitoring setup
- [ ] IPv6 dual-stack implementation

### Advanced Features
- [ ] Software-Defined Networking (SDN)
- [ ] Network automation scripts
- [ ] Security incident response procedures
- [ ] Disaster recovery planning

## 📚 Educational Objectives

This project demonstrates:
- Hierarchical network design principles
- VLAN implementation and management
- Inter-VLAN routing configuration
- Spanning Tree Protocol (STP)
- Network troubleshooting methodologies
- Enterprise network best practices

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -am 'Add new feature'`
5. Push to the branch: `git push origin feature-name`
6. Submit a pull request

### Contribution Guidelines
- Test all configurations before submitting
- Document any new features or changes
- Follow Cisco configuration best practices
- Update README if adding new components



## 👥 Authors

- **Your Name** - *Initial work* - [YourGitHub](https://github.com/RAJMadhusankha)

## 🙏 Acknowledgments

- Cisco Networking Academy for educational resources
- Network design best practices from enterprise implementations
- Community feedback and contributions

## 📞 Support

For questions or support:
- Open an issue on GitHub
- Email: your.janithm2000@gmail.com
- LinkedIn: [Your Profile](www.linkedin.com/in/janithmadusankha)

---

**⭐ If you find this project helpful, please give it a star!**

*Last updated: August 2025*
