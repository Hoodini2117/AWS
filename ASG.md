# AUTO SCALING GROUP

Running virtual machines in the cloud is made possible by Amazon EC2 (Elastic Compute Cloud). However, manually managing these instances can be inefficient and time-consuming, especially when dealing with changing workloads. This is where Auto Scaling proves valuable—it allows your infrastructure to automatically adjust to fluctuations in demand.

With Auto Scaling Groups (ASG), you can ensure that the right number of EC2 instances are running based on specific conditions such as CPU utilization or incoming traffic. Auto Scaling handles the addition or removal of instances automatically, maintaining your desired capacity to keep applications available and responsive.

The process begins with creating an Amazon Machine Image (AMI)—a snapshot of an EC2 instance that serves as a reusable template for launching new instances. Next, you define Launch Configurations or Launch Templates, which specify the instance type, AMI, and security groups to be used for newly launched EC2 instances.

ASGs can be configured to scale dynamically using real-time monitoring tools like CloudWatch alarms. For example, if CPU usage exceeds 80% for a set duration, the ASG will launch additional instances to distribute the load. Conversely, if CPU usage falls below a certain threshold, it will terminate unneeded instances to reduce costs.

![Screenshot 2025-05-27 013514](https://github.com/user-attachments/assets/18882691-f392-42f0-b060-838c272b7cac)
![Screenshot 2025-05-27 013743](https://github.com/user-attachments/assets/0b3409bd-600a-4706-92fa-f97d9ced73cf)
![Screenshot 2025-05-27 013810](https://github.com/user-attachments/assets/21ee9fba-2482-49c2-80d6-8b2c50991467)
