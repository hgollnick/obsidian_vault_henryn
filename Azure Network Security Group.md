[[Azure]]

In Microsoft Azure, a Network Security Group (NSG) is a fundamental component of network security that allows you to control inbound and outbound traffic to resources deployed in an [[Azure Virtual Network]]] (VNet). NSGs act as a virtual firewall and provide a way to define rules that permit or deny traffic based on attributes such as source IP address, destination IP address, port, and protocol.

Key features and concepts associated with Azure Network Security Groups include:

1. **Rules:** NSGs consist of a set of inbound and outbound security rules. Each rule defines a specific set of criteria for allowing or denying traffic. Rules are processed in priority order, and the first matching rule determines the action to be taken.
    
2. **Default Rules:** By default, an NSG includes a set of default rules that allow outbound traffic and deny inbound traffic. These default rules can be customized or overridden with user-defined rules.
    
3. **Associating NSGs:** NSGs can be associated with subnets ([[Azure Subnet]]), individual network interfaces, or even directly with virtual machines. When associated with a subnet, the NSG rules apply to all resources within that subnet.
    
4. **Rule Components:** NSG rules consist of the following components:
    
    - **Name:** A user-defined name for the rule.
    - **Priority:** An integer value that determines the order in which rules are processed. Lower numbers indicate higher priority.
    - **Source/Destination:** Defines the source or destination of the traffic based on IP address, service tag, or application security group.
    - **Port and Protocol:** Specifies the port number and protocol (TCP, UDP, or Any).
    - **Action:** Specifies whether to allow or deny traffic.