# Lab 3 - Switch Configuration & VLANs

## Objective
Configure a Cisco Router Configuration – Connecting Two Networks.

Router interfaces
IP addressing
Subnet masks
Default gateways
Directly connected networks
Routing table
Interface status
Ping troubleshooting
Cisco IOS configuration
Saving router configuration

## Devices
- 2 PCs
- 2 Cisco 2960 Switch
- 1 Router 1941

## Router Configuration Performed
- enable	            //Enter privileged mode
- configure terminal	//Enter configuration mode
- interface g0/0	    //Select interface
- ip address	        //Assign IP address
- no shutdown	        //Enable interface
- show ip interface brief	//Check interface status/IPs
- show ip route	        //View routing table
- ping	                 //Test connectivity
- copy running-config startup-config	//Save configuration

## Verification
- show interfaces status
- show running-config

## Result
Configured Cisco router interfaces to connect multiple IPv4 networks and verified inter-network connectivity using ping and routing-table commands.