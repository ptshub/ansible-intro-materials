Per ESXi Host:

Set iLo address:
	-IP
	-Subnet
	-Gateway (if needed)
Set Network Adapters
	-vmnic0: Set vmnic variable: "Connected" 
	-vmnic1: Set vmnic variable: "Connected"
Set ESXi IP address:
	-IP
	-Subnet
	-Gateway
Set ESXi DNS server:
	-IP
	-Subnet
	-Gateway
Set ESXi NTP server:
	-Enable NTP service
	-Set NTP IP address
	-Start NTP service
	-Set NTP service variable: "Start and Stop with host"

<<<<<<<<<VSS Switch>>>>>>>>>
Add VSAN portgroup to vSwitch0
Add VSAN IP to ESXi
	-IP Address
	-Subnet
	-Gateway (if needed)

Add VSAN IP address to VSAN portgroup
Add vmk(x) for VSAN Network

On vCenter:
Create VSAN Cluster on vCenter
	-DRS enable
	-HA enable
	-VSAN service enable

Add ESXi Hosts to VSAN Cluster

Claim Disks