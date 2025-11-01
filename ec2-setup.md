EC2 Setup (manual) Launch EC2 instances (Amazon Linux 2 or Ubuntu 22.04)

Backend: Launch 2 instances (t3.micro or t2.micro) Frontend: Launch 1 instance Attach appropriate security groups (see security-groups.md)

Connect via SSH:

ssh -i your-key.pem ec2-user@PUBLIC_IP Install prerequisites manually or use deployment scripts in /deployment.
