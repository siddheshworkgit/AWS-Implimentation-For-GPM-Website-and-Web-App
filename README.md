#Architectural Summary :

PHP Website hosted on EC2 in Private Subnet

RDS (MySQL/PostgreSQL) in another Private Subnet

Bastion Host in Public Subnet for secure access

NAT Gateway for Private Subnet EC2 to access internet (for fetching CDN assets)

Application Load Balancer (ALB) in front

Multi-AZ + Cross-Region setup for High Availability and DR

Route 53 for DNS

S3 + CloudFront as CDN (optional, for static assets)

Auto Scaling Group for EC2

Security Groups + NACLs for protection
