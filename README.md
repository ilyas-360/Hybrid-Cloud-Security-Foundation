# Enterprise Secure Hybrid Infrastructure (CCNA Mega-Lab)

## 🎯 Strategic Objective

This repository documents a high-availability, multi-site enterprise network
designed as a **secure foundational underlay** for Hybrid Cloud and
Identity-centric architectures.

The lab mirrors real-world enterprise design patterns used to securely connect
on-premises infrastructure to Cloud Identity Providers such as
Microsoft Entra ID (Azure AD) and AWS IAM, emphasizing **segmentation,
redundancy, and the Principle of Least Privilege (PoLP)**.

---

## 🛡️ Security & Identity-Oriented Design

While aligned with CCNA objectives, this implementation prioritizes
**Zero Trust concepts** commonly used in modern enterprise and cloud environments:

- **Zero Trust Foundations**
  - Port Security and DHCP Snooping establish basic endpoint trust signals
    (MAC/IP bindings), reducing rogue device participation.

- **Micro-Segmentation**
  - VLAN-based isolation enforces workload separation and maps directly to
    Cloud Network Security Group (NSG) design principles.

- **Privileged Access Management (PAM)**
  - Management-plane ACLs and SSHv2 restrict administrative reachability to
    explicitly authorized management sources only.

---

## 🛠️ Technical Implementation

- **High Availability**
  - HSRP provides first-hop redundancy at the distribution layer.
  - EtherChannel (LACP) ensures link-level resilience between critical devices.

- **Scalability**
  - Hierarchical Core / Distribution / Access architecture supports enterprise
    growth and operational clarity.

- **Edge Connectivity**
  - Single-area OSPF for dynamic routing.
  - NAT/PAT at the edge for controlled and auditable internet access.

---

## 📁 Repository Structure

```plaintext
configs/             # Hardened device configurations (Core, Distribution, Access, Edge)
design-docs/         # Addressing plans and segmentation logic
identity-security/   # Least Privilege and management-plane security design
verification/        # Connectivity audits and security validation evidence

Ilyas Benkhadra
Cybersecurity & Cloud Identity Engineering
