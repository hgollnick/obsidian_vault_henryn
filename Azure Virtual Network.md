[[Azure]]

In Microsoft Azure, a Virtual Network (VNet) is a fundamental building block that enables you to create private, isolated networks in the cloud. Azure VNets allow you to securely connect Azure resources, such as virtual machines (VMs), to each other, to on-premises networks, and to the internet. Here are key features and concepts associated with Azure Virtual Networks:

1. **IP Addressing:**
    
    - VNets are associated with one or more IP address ranges specified in CIDR notation. These address ranges define the private IP space available to resources within the VNet.
    - Subnets are created within the VNet, and each subnet is associated with a specific IP address range.
2. **Subnets:**
    
    - Subnets are logical subdivisions of a VNet, and they help organize and segment resources within the VNet. Resources in different subnets can communicate with each other based on network configurations.

There are also some concepts used such as:

1. **Azure Bastion:**
    
    - Azure Bastion is a service that allows secure and seamless RDP and SSH access to VMs directly from the Azure portal over the Azure Backbone network.
2. **Azure Virtual Network Gateway:**
    
    - The Virtual Network Gateway enables site-to-site VPN and ExpressRoute connections. It acts as a gateway for secure communication between on-premises networks and Azure VNets.