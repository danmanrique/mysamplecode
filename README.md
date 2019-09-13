# mysamplecode
Place to store my sample code


Azure - CreateNetwork Folder:
This folder contains a template file, parameter file and cli code for building out a baseline hybrid network. It contains a hub vnet, a spoke vnet, and a simulated on-premise vnet. 

The hub contains multiple subnets (GatewaySubnet, AzureFirewallSubnet, ManagementSubnet), with an Azure Firewall in the AzureFirewallSubnet, and a jumpbox in the Managementsubnet. 
The spoke contains two subnets (GatewaySubnet, SN-Workload) and a vm running iis in the SN-Workload subnet. 
The on-premise network has a GatewaySubnet and a SN-Corp subnet with a vm (to test client to spoke connectivity).

There are virtual network gateways (site-to-site vpn), and UDRs in the route tables. There is LogAnalytics for diagnostics data on the FW. There is a KeyVault deployed, but no secrets in it. 

The intent for me was to have an environment I could spin up at any time to test connectivity, monitoring and security scenarios.
I built this somewhat based on the tutorial: https://docs.microsoft.com/en-us/azure/firewall/tutorial-hybrid-portal


