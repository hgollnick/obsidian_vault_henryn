[[Azure]]

There are several types of IP addresses in Azure, each serving a specific purpose. Here are some key types of IP addresses in Azure:

1. **Public IP Address:**
    
    - A Public IP address is used for communication over the internet. It can be associated with resources such as Azure Virtual Machines, Load Balancers, Application Gateways, or [[Azure Network Interface]].
    - Public IP addresses can be either dynamically or statically assigned. Statically assigned public IPs are typically used for scenarios where a fixed, public-facing IP address is required.
2. **Private IP Address:**
    
    - A Private IP address is assigned to resources within an [[Azure Virtual Network]] for communication within the network or with connected networks through VPN or ExpressRoute.
    - Virtual Machines and Network Interfaces in Azure can have one or more private IP addresses associated with their NICs and configurations.
3. **Dynamic IP Address Assignment:**
    
    - Dynamic IP address assignment is a method where IP addresses are automatically assigned by Azure. This is often used for private IP addresses within a Virtual Network.
4. **Static IP Address Assignment:**
    
    - Static IP address assignment allows you to specify a fixed IP address for a resource. This is commonly used for scenarios where a resource needs a consistent and unchanging IP address.
5. **Reserved IP Addresses:**
    
    - Azure allows you to reserve a specific IP address within a Virtual Network. This ensures that the IP address is not used by other resources, even if the resource associated with it is deallocated or deleted.