# azure-beginner-cloud-project
Step-by-step Azure cloud infrastructure build with VM, storage, CI/CD, and monitoring
---

Phase 1: Azure Environment Setup

This phase involved creating the foundation of the cloud infrastructure, including networking and firewall configurations.

  What I Built
- [x] Resource Group: `BeginnerCloudRG`
- [x] Virtual Network: `BeginnerVNet` with address space `10.0.0.0/16`
- [x] 4 Subnets:
  - `WebSubnet1` – `10.0.1.0/24`
  - `WebSubnet2` – `10.0.2.0/24`
  - `DBSubnet1` – `10.0.3.0/24`
  - `DBSubnet2` – `10.0.4.0/24`
- [x] NSGs:
  - `WebNSG` with rules for HTTP, HTTPS, SSH
  - `DBNSG` with no public inbound rules
- [x] Applied correct NSGs to subnets

![vnet-subnets](https://github.com/user-attachments/assets/81a3e00f-0135-4317-aaa6-00fdf961d5fb)

![webnsg-rules](https://github.com/user-attachments/assets/7a3b4041-2e36-45f7-8b2c-ec3bcb098898)

![subnet-nsg-link](https://github.com/user-attachments/assets/e458f55a-3490-4464-aa7e-c985f2ef27cd)

