# mysamplecode
Place to store my sample code


Azure - CreateNetwork Folder:
This folder contains a template file, parameter file and cli code for building out a baseline hybrid network. It contains a hub vnet, a spoke vnet, and a simulated on-premise vnet. 

The hub contains multiple subnets, and an Azure Firewall. There is a jumpbox in an management subnet. 
The spoke contains a vm running iis. 
The on-premise network has a vm.

The intent for me was to have an environment I could spin up at any time to test connectivity, monitoring and security scenarios.
I built this based on the tutorial: https://docs.microsoft.com/en-us/azure/firewall/tutorial-hybrid-portal


