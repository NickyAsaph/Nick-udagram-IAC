Deploy a High-Availability Web Application (Udagram APP) Using AWS CloudFormation
project_URL: http://nick-WebAp-1XGZMO6EWK44O-691433579.us-west-2.elb.amazonaws.com 

This Project is an Instagram-Like App Infrastructure-as-code (IAC) deployment Called UDAGRAM. The purpose is to automates the process of creating a secured and high-availability environment, and deploying an application into an Apache Web Server. The script contains all the configurations needed for a repeatable process so that the infrastructure can be discarded and recreated at will multiple times. Features 1 - Load-balanced servers with auto-scaling capability across two availability zones In a single region.

2 - Ec2 instance specification: 2vCPUs, 4GB RAM, 10GB Ebs storage.

3 - Ubuntu 18 Operating System using Amazon machine image.

4 - Compute Ec2 instances are secured in a private subnet and only accepts traffic originating load-balancer within the public subnet.

5 - Elastic Load-balancer and application servers have security groups defined with only required ports opened.

6 - Application servers have outbound internet access via NAT gateway for critical OS updates and patches.

7 - Application servers are configured with IAM instance profile to be able to access and download application code from AWS S3 bucket.

8 -Health checks and thresholds are defined to aid in system availability detection.

9 - Entire environment is fully virtualized in a cloud platform that can be taken down and brought back up within a short period of time. The process of creating and starting all the services, spinning up instances are automated via scripts in this repo.

Infrastructure Architectural Diagram
![Nick-udagram](https://user-images.githubusercontent.com/87441050/174900410-9248908a-34ab-4f77-bf57-658d082ec069.png)
