# BASTION HOST

Amazon EC2 (Elastic Compute Cloud) is one of AWS’s core services, allowing you to run virtual servers—essentially remote computers—in the cloud that you can start, stop, configure, and scale as needed. However, in real-world deployments, not all EC2 instances are exposed directly to the internet for security reasons. This is where the concept of a Bastion Host comes into play.

A Bastion Host is a publicly accessible EC2 instance that acts as a secure gateway to access private EC2 instances within a Virtual Private Cloud (VPC). To set this up, the Bastion Host is placed in a public subnet connected to an Internet Gateway (IGW), enabling SSH access from your local machine. The EC2 instance you intend to access is located in a private subnet, which remains isolated from direct internet exposure.

configuring a bastion host includes several steps :- 

### create vpc
https://cdn.discordapp.com/attachments/843880824696471552/1376810479850360892/image.png?ex=68413a2e&is=683fe8ae&hm=0f2d75666ed3ab9b98697a16f970d025e3bd7ee97a012894d2dd681507bb50d0&
