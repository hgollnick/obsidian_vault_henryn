[[Azure]]

In Microsoft Azure, a subnet is a range of IP addresses in your [[Azure virtual network]] (VNet). Azure subnets are used to divide a VNet into smaller, more manageable segments. Each subnet represents a grouping of resources, and it can be associated with specific network security and routing configurations. Subnets play a crucial role in organizing and controlling network traffic within an Azure VNet.

Key characteristics and functions of Azure subnets include:

1. **IP Address Range:** A subnet is defined by an IP address range within the overall address space of the VNet. The IP address range is specified in CIDR (Classless Inter-Domain Routing) format.
    
2. **Resource Group Association:** Subnets are created within an Azure resource group and associated with a specific VNet. This association allows you to organize and manage resources effectively.
    
3. **Network Isolation:** Resources within a subnet can communicate with each other directly without going through a network gateway. However, by default, communication between subnets is not allowed unless explicit peering or network security group rules are configured.
    
4. **Security and Routing:** Subnets provide a boundary for network security and routing. Network Security Groups (NSGs) can be associated with subnets to control inbound and outbound traffic, and route tables can define how traffic is routed between subnets.
    
5. **Azure Virtual Machines (VMs):** When you deploy Azure VMs, you typically place them within specific subnets. Each VM gets an IP address from the subnet's IP range.