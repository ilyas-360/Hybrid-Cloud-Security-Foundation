# Hybrid Cloud Security Foundation: Enterprise Networking for AWS Connectivity

🎯 **Objective**
Secure high-availability enterprise network designed to bridge on-premises infrastructure with AWS Cloud. Focused on traffic segmentation, high-speed connectivity, and Principle of Least Privilege (PoLP).

🛡️ **AWS Security & Infrastructure Alignment**
- **Zero Trust Underlay:** Port Security and DHCP Snooping establish hardware trust signals.
- **Infrastructure Segmentation:** VLAN isolation mapped to AWS Security Groups & NACLs.
- **Hardened Management Plane:** Restricted SSHv2 + ACL-based admin access, simulating AWS Site-to-Site VPN & Direct Connect security.

🛠️ **Technical Implementation**
- High Availability: HSRP + EtherChannel (LACP)
- Hybrid Routing: OSPF with preparation for BGP peering to AWS
- Traffic Egress: NAT/PAT with logging for CloudWatch-like audits

📁 **Repository Structure**
- `configs/` - Core, Distribution, Access, Edge device configurations
- `design-docs/` - Addressing plans and hybrid cloud design
- `security-control-plane/` - Management plane hardening & policies
- `verification/` - Connectivity audits & security validation
- `future-aws-integration/` - Terraform modules & VPN setup

🚀 **Planned AWS Integration**
1. Site-to-Site VPN from Edge Router to AWS VPC  
2. Terraform IaC for hybrid cloud deployment  

**Ilyas Benkhadra**  
*Cloud Security Engineer | AWS Infrastructure & Network Hardening*

