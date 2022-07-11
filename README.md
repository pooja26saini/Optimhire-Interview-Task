The Script is adding a port 443 as an incoming rule. If want to make it an outgoing rule then use "egress" as an type.

Following are the parameters used :

1. from_port - (Required) Start port (or ICMP type number if protocol is "icmp" or "icmpv6").

2. protocol - (Required) Protocol. If not icmp, icmpv6, tcp, udp, or all use the protocol number

3. security_group_id - (Required) Security group to apply this rule to.

4. to_port - (Required) End port (or ICMP code if protocol is "icmp").

5. type - (Required) Type of rule being created. Valid options are ingress (inbound) or egress (outbound).

6. cidr_blocks - (Optional) List of CIDR blocks. Cannot be specified with source_security_group_id or self.

7. description - (Optional) Description of the rule.

8. ipv6_cidr_blocks - (Optional) List of IPv6 CIDR blocks. Cannot be specified with source_security_group_id or self.

9. prefix_list_ids - (Optional) List of Prefix List IDs.

10. self - (Optional) Whether the security group itself will be added as a source to this ingress rule. Cannot be specified with cidr_blocks, ipv6_cidr_blocks, or source_security_group_id.

11. source_security_group_id - (Optional) Security group id to allow access to/from, depending on the type. Cannot be specified with cidr_blocks, ipv6_cidr_blocks, or self.
