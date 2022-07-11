The Script is adding a port 443 as an incoming rule. If want to make it an outgoing rule then use "egress" as an type.

from_port - (Required) Start port (or ICMP type number if protocol is "icmp" or "icmpv6").

protocol - (Required) Protocol. If not icmp, icmpv6, tcp, udp, or all use the protocol number

security_group_id - (Required) Security group to apply this rule to.

to_port - (Required) End port (or ICMP code if protocol is "icmp").

type - (Required) Type of rule being created. Valid options are ingress (inbound) or egress (outbound).

cidr_blocks - (Optional) List of CIDR blocks. Cannot be specified with source_security_group_id or self.

description - (Optional) Description of the rule.

ipv6_cidr_blocks - (Optional) List of IPv6 CIDR blocks. Cannot be specified with source_security_group_id or self.

prefix_list_ids - (Optional) List of Prefix List IDs.

self - (Optional) Whether the security group itself will be added as a source to this ingress rule. Cannot be specified with cidr_blocks, ipv6_cidr_blocks, or source_security_group_id.

source_security_group_id - (Optional) Security group id to allow access to/from, depending on the type. Cannot be specified with cidr_blocks, ipv6_cidr_blocks, or self.
