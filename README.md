# azure-beginner-cloud-project
Hands-on Azure cloud project covering core infrastructure: networking, virtual machines, storage, CI/CD pipelines, and monitoring — fully deployed in the Azure Portal.

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

[Cloud Build Tracker Project Board] https://github.com/users/Idirisahmed05/projects/2

---

Phase 2: Windows VM + IIS Web Server

- [x] Deployed Windows Server 2022 VM in WebSubnet1
- [x] Connected via RDP
- [x] Installed IIS using PowerShell or Server Manager
- [x] Served a custom index.html page

VM Overview:
![WinWebVM] ![WinWebVM](https://github.com/user-attachments/assets/f1894d8b-0f19-4831-a919-73114b62a91a)



Live Web Page:
![Web Page] ![Html](https://github.com/user-attachments/assets/dd0ec92f-3bcf-4c41-88bf-b8c82a834f33)
