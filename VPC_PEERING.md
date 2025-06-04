# VPC PEERING

A virtual private cloud (VPC) is a virtual network dedicated to your AWS account. It is logically isolated from other virtual networks in the AWS Cloud. You can launch AWS resources, such as Amazon EC2 instances, into your VPC.

A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them using private IPv4 addresses or IPv6 addresses. Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your own VPCs, or with a VPC in another AWS account. The VPCs can be in different Regions (also known as an inter-Region VPC peering connection).
AWS uses the existing infrastructure of a VPC to create a VPC peering connection; it is neither a gateway nor a VPN connection, and does not rely on a separate piece of physical hardware. There is no single point of failure for communication or a bandwidth bottleneck.

A VPC peering connection helps you to facilitate the transfer of data. For example, if you have more than one AWS account, you can peer the VPCs across those accounts to create a file sharing network. You can also use a VPC peering connection to allow other VPCs to access resources you have in one of your VPCs.

### create two vpc
![Screenshot 2025-05-30 174259](https://github.com/user-attachments/assets/5711c503-a532-4a3a-a7f2-0dcd669ac755)

### create two subnets
![Screenshot 2025-05-30 174303](https://github.com/user-attachments/assets/286f342d-70de-47d2-aa84-24e9e9091701)

### create two ec2 isntances
![Screenshot 2025-05-30 174246](https://github.com/user-attachments/assets/87556800-f6f2-45ad-b962-9793517403ee)

### add route tables to the subnets
![Screenshot 2025-05-30 174327](https://github.com/user-attachments/assets/741fb91e-5bc5-413e-83f9-d2fc3c5e3066)

## configure a peering connection
![Screenshot 2025-05-30 174339](https://github.com/user-attachments/assets/ebe467d0-63da-4ac0-9f04-8e0e7b145766)

### after all the steps, ssh into each ec2 of the different vpc's
![Screenshot 2025-05-30 174238](https://github.com/user-attachments/assets/0596cea4-6b92-4bea-9846-1b2b262fd9ca)

