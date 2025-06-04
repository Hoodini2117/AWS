# BASTION HOST

Amazon EC2 (Elastic Compute Cloud) is one of AWS’s core services, allowing you to run virtual servers—essentially remote computers—in the cloud that you can start, stop, configure, and scale as needed. However, in real-world deployments, not all EC2 instances are exposed directly to the internet for security reasons. This is where the concept of a Bastion Host comes into play.

A Bastion Host is a publicly accessible EC2 instance that acts as a secure gateway to access private EC2 instances within a Virtual Private Cloud (VPC). To set this up, the Bastion Host is placed in a public subnet connected to an Internet Gateway (IGW), enabling SSH access from your local machine. The EC2 instance you intend to access is located in a private subnet, which remains isolated from direct internet exposure.

configuring a bastion host includes several steps :- 

### create vpc
![image](https://github.com/user-attachments/assets/a3a69d59-63b5-4651-b394-1ef29dc386d8)

### create public and private subnets 
![image](https://github.com/user-attachments/assets/ab97ad8e-4216-48d1-a6fc-a67f6df69ac3)

### create internet gateway
![image](https://github.com/user-attachments/assets/b497f124-0d7b-46ca-aec3-b174ac93971c)

add route tables to the IGW
![image](https://github.com/user-attachments/assets/9af79cdd-8324-4ef6-8b27-4646e3de2a8e)


from the bastion host..ssh into the private ec2
![image](https://github.com/user-attachments/assets/dc83458e-9420-424d-8791-8459f9df422c)
