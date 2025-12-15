# Objective: Get hands-on with compute by starting a small EC2 instance and connecting via SSH (or RDP).

## Prerequisites: IAM user with EC2 access; security group basics

### Steps:

1. Open EC2 service → Launch Instance.
2. Choose an AWS Free Tier eligible AMI (e.g., Ubuntu Server 20.04 LTS).
3. Choose an instance type: t2.micro (or t3.micro in newer regions) and continue.
4. Configure:
  Instance details: default is fine
  Add Storage: default 8 GB is fine
  Add Tags: Name = lab-ec2
  Configure Security Group: allow SSH (port 22) from your IP (recommended); you can also enable HTTP for a simple web test (optional)
5. Review and Launch. Create/select a key pair (e.g., lab-key.pem), download it, and set permissions (chmod 400).
6. Connect to the instance using SSH:
  ssh -i lab-key.pem ubuntu@<PublicDNS-or-IP>
7. (Optional) Install a simple web server:
  sudo apt update && sudo apt install -y nginx
  sudo systemctl start nginx
  Visit the public IP in a browser to see the default Nginx page.

## Expected Results:

Instance launches and is reachable via SSH (and HTTP if enabled).

## Assessment / Checklist:

1. Instance launched in free tier region
2. Security group configured to allow SSH from your IP
3. Successful SSH connection (and optional HTTP access)
