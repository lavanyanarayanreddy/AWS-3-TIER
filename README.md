# AWS-3-TIER

AWS 3 Tier Application Architecture
This project demonstrates the implementation of a highly available, scalable, and secure 3-tier web application architecture using Amazon Web Services (AWS). The architecture consists of three primary layers: Web (Public), Application (Private), and Database. The solution ensures fault tolerance and scalability by leveraging AWS services such as EC2, RDS, Elastic Load Balancer (ALB), Auto Scaling, and CloudWatch.



Components:
Amazon EC2: Hosting application servers.
Amazon RDS: Managed MySQL database for storing WordPress data.
Elastic Load Balancer (ALB): Distributes traffic to ensure high availability and scalability.
Auto Scaling: Ensures that the number of application instances adjusts based on demand.
NAT Gateway & Internet Gateway: Enable secure communication between private subnets and the internet.

Key Features:
VPC Setup: A custom VPC with public and private subnets across multiple Availability Zones (AZs) for high availability.
Application Load Balancer (ALB): Distributes incoming traffic across multiple EC2 instances for better availability and fault tolerance.
Auto Scaling: Automatically adjusts the number of EC2 instances based on incoming traffic, ensuring efficient resource utilization.
Security: Configured Security Groups and IAM roles to control access and ensure secure communication between components.
RDS Database: Set up a multi-AZ MySQL database for high availability and data durability.
WordPress Deployment: Deployed a WordPress application on EC2 instances with Apache HTTPD, PHP, and MariaDB.
Monitoring and Alerts: Integrated Amazon CloudWatch for monitoring the performance and health of the infrastructure and set up SNS for real-time alerts.

Architecture:
The architecture includes a custom VPC with segregated subnets for public and private access, multiple AZs for redundancy, and integrated monitoring to ensure the application remains available under varying loads.
