# Multi-Cloud Weather Tracker with Disaster Recovery

![Architecture Diagram Placeholder](images/architecture-diagram.png)

## Overview
This project deploys a weather tracking application across AWS and Azure with disaster recovery. Terraform automates multi-cloud provisioning, while Route 53 DNS failover ensures high availability. It demonstrates multi-cloud deployment, resilience, and automation for production-ready applications.

## Problem Statement
Single-cloud hosting is vulnerable to outages and downtime. Manual failover management is complex and error-prone. The challenge was to design an automated multi-cloud solution capable of maintaining service continuity, high availability, and global scalability.

## Solution
- Host front-end on AWS S3 with CloudFront and Azure Blob Storage  
- Automate infrastructure with Terraform for repeatable deployments  
- Configure Route 53 DNS failover between AWS and Azure endpoints  
- Monitor health of endpoints and automatically redirect traffic if a cloud fails  

![Workflow / Implementation Placeholder](images/workflow.png)

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
![Application Screenshot Placeholder](images/results.png)  

## Future Improvements
- Integrate automated backups and monitoring  
- Add multi-region failover for enhanced resiliency  
- Implement serverless backend for dynamic weather analytics  
