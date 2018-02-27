# CS435 Repository
This repository contains material for the  [CS435](www.csd.uoc.gr/~hy435 "CS435") course. 

## Network devices configuration 
The `configs` directory contains the default configurations for the available network equipement. Remember to apply the configuration on the proper device, to avoid confusion. 

### Network topology 
For easilly accessing the available network devices a management VLAN is configured (VLAN ID: 1000).  This VLAN is on the `192.168.4.1/24` subnet. For all the available routers the management VLAN is configured in the `eth0` port, whereas for the `EdgeSwitch 8` on the port `1`.  You can access the VLAN from a non-tagged host using the port `24` of the EdgeSwitch `24`, which is automatically performs tagging with the management VLAN ID. For your convinience, there is a `DHCP` running on this VLAN which will automatically provide a proper address on the connected host.

To avoid confusion and problems that may arise from misconfiguration, let's assume that no team is allowed to edit the configuration parameters of the management ports. If you do so, please revert your changes before leaving the lab, or just upload the default configurations provided. 
