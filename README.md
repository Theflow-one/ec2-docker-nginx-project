# ec2-docker-nginx-project
My first Cloud/DevOps project: Building a containerized web server from scratch on AWS. Includes automated deployment scripts and a focus on moving from learning to secure production standards

Project Genesis: Secure AWS & Docker Deployment
My Project Overview
This project represents my first deep dive into Cloud Infrastructure and Containerization and its challenges. I built a custom Cloud Sandbox on AWS and deployed a live Nginx web server using Docker the main goal was to understand the process and the importance of the correct security measures not just to click buttons blindly.

The Journey 
I started this project with some knowledge of AWS VPCs and EC2 but cero Docker. Through this process, I moved from basic setup to understanding professional-grade security although theres much i need to learn it was refreshing the amoung of knowledge gained.

Phase 1: Infrastructure (The Genesis)

Custom VPC: Built a private network with a custom IPv4 CIDR.

Networking: Configured the Internet Gateway and Route Tables to allow traffic.

Troubleshooting: I successfully resolved a VPC Subnet conflict by recalculating my IP ranges when I hit an overlap error which solidify the understanding of CIDR.

Phase 2: Containerization & Security

Automation: Created a deploy.sh script to handle system updates and Docker deployment automatically.

Hardening: Configured AWS Security Groups to restrict all traffic specifically to my personal IP seeing that in the deployment of the ec2 yesterday to the open internet the amount of cyber attacks was eye opening which establish a deeper respect for security measures when deploying to live productions.

Identified and fixed a Docker Credential vulnerability by moving from plain-text storage to an encrypted GPG-vault (pass), the message the docker dispayed concerning the credential raised a alarm which lead me to follow up with the json settings before continuing with my original plan.

Performed security scanning using Docker Scout, after downloading the correct pluggings to terminal and having the correct credentials.

AI Collaboration Disclosure
I want to be transparent that I used AI, which as a technical assistant for this project.

The AI's Role: Provided explanations for complex topics like CIDR notation and helped format my deployment script.

My Role: I performed every step manually, handled all real-world troubleshooting (like the IP changes and network glitches), and verified every security patch. Plus doble checked all the outputs by the ai assistence to make sure i was following protocol, there were times that i had to redirect the flow of the process to keep a logical structure.

Using AI allowed me to learn a month's worth of material in a few days, but the engineering and execution are 100% my own work and have realistic expectations to understand its value as a assistan.

