# Multi-Cloud Weather Tracker with Disaster Recovery

<p align="center">
  <img src="https://i.gyazo.com/1e5d79c85a1e37f2a0e01f4df5d0e7ec.png" alt="Diagram" width="700">
  <br>
  <sub>Figure 1: Architecture Diagram</sub>
</p>

## Overview
This project deploys a weather tracking application across AWS and Azure with disaster recovery. Terraform automates multi-cloud provisioning, while Route 53 DNS failover ensures high availability. It demonstrates multi-cloud deployment, resilience, and automation for production-ready applications.

## Problem Statement
Single-cloud hosting is vulnerable to outages and downtime. Manual failover management is complex and error-prone. The challenge was to design an automated multi-cloud solution capable of maintaining service continuity, high availability, and global scalability.

## Solution
- Host front-end on AWS S3 with CloudFront and Azure Blob Storage  
- Automate infrastructure with Terraform for repeatable deployments  
- Configure Route 53 DNS failover between AWS and Azure endpoints  
- Monitor the health of endpoints and automatically redirect traffic if a cloud fails  

<table align="center">
  <tr>
    <td colspan="2" align="center">
      <img src="https://i.gyazo.com/ef77549526ea2f286dd4201f39928ff7.png" alt="S3" width="600">
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://i.gyazo.com/21f71ccae069d27179503a23726f96db.png" alt="Repeatable deployment" width="600">
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://i.gyazo.com/0822cf8599d2792524983637f7ff2705.png" alt="Primary Record" width="350">
    </td>
    <td align="center">
      <img src="https://i.gyazo.com/2f4aae960f45be4881459a6e0e4c7aca.png" alt="Secondary" height="250">
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <sub>Figure 2: Workflow</sub>
    </td>
  </tr>
</table>

## Steps to be Performed 👩‍💻
1. Install Terraform, AWS CLI, Azure CLI  
2. Define AWS Resources in Terraform  
3. Define Azure Resources in Terraform  
4. Implement Disaster Recovery with Route 53 Failover  

## Key Services / Tools Used 🛠
- AWS S3 [Hosting]  
- AWS CloudFront [CDN]  
- Azure Blob Storage [Hosting]  
- Route 53 [DNS Failover]  
- Terraform [Infrastructure as Code]  

## Results

<p align="center">
  <img src="https://i.gyazo.com/4b4e6e9bb2f0f6d0020d9879ce6e913c.png" alt="Application" width="700">
  <br>
  <sub>Figure 3: Application</sub>
</p>

## Future Improvements
- Integrate automated backups and monitoring  
- Add multi-region failover for enhanced resiliency  
- Implement serverless backend for dynamic weather analytics  
