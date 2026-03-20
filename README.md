# AWS Auto Scaling Load Balanced Architecture

## Project Overview
This project demonstrates a highly available AWS web architecture using an Application Load Balancer, Target Group, Launch Template, and Auto Scaling Group.

## Architecture
Internet
   |
Application Load Balancer
   |
Target Group
   |
Auto Scaling Group
   |
EC2 Instances

## Technologies Used
- AWS EC2
- AWS Application Load Balancer
- AWS Target Groups
- AWS Auto Scaling Groups
- AWS Launch Templates
- Ubuntu Linux
- Nginx

## What I Configured
1. Created EC2 web servers
2. Added them behind an Application Load Balancer
3. Created a launch template with user data to install Nginx automatically
4. Created an Auto Scaling Group across two Availability Zones
5. Attached the Auto Scaling Group to the target group
6. Troubleshot unhealthy targets and corrected the launch template/user data
7. Confirmed the load balancer served the Auto Scaling instances successfully

## Key Concepts Learned
- Load balancing
- Target groups
- Health checks
- Launch templates
- Auto Scaling Groups
- Fault tolerance
- Automated recovery

## Result
The environment serves traffic through an Application Load Balancer to Auto Scaling EC2 instances running Nginx.
