# path based routing using ALB

The Application Load Balancer (ALB) is a powerful traffic management service provided by *Amazon Web Services (AWS). It is designed to route HTTP and HTTPS traffic to your target resources based on request attributes such as URL paths, host headers, or query strings. One of its commonly used features is *Path-Based Routing, which directs incoming requests to different target groups depending on the URL path.

For example, if you have multiple applications running in separate environments (like /APPLICATION_A and /AAPLICATION_B), the ALB can route traffic to the appropriate backend resources (such as EC2 instances) based on these specified paths.

 You can use an Application Load Balancer to create a listener with rules that forward requests to target groups based on the URL. The path pattern rules apply only to the path of the URL and not to the query parameters of the URL. For more information about path patterns, see Path conditions.

Note: This feature isn't supported for Classic Load Balancer, Network Load Balancer, or Gateway Load Balancer.

To establish path-based routing on your Application Load Balancer, complete these steps:
Create a target group.
Configure listener rules.

create two ec2 instances with webservers , (here - apache and nginx)
![image](https://github.com/user-attachments/assets/883f1f7a-20b9-4087-8dac-e20cd5a56d4d)

create target groups (here nginx-tg and apache-tg)
![image](https://github.com/user-attachments/assets/9d4cc313-e91c-47e6-bb2c-60b4fdc826fc)

configure an application load balancer with listener rules (default routes to /apache)
![image](https://github.com/user-attachments/assets/5a4c80bf-7b38-46de-9bb7-eace9a0cfc3a)

![image](https://github.com/user-attachments/assets/f237f0dc-954d-4901-9243-9bb19a6b5b41)

![image](https://github.com/user-attachments/assets/a4bc88f0-bbf4-4e6b-8ca8-7dd694d4c255)

routes to /nginx when specified and to /apache as default or if specified as apache.


