# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: YASVANTH D
* **Register Number**: 212223090031
* **Date of Submission**: 26/02/26

---

## Objective

The objective of this experiment is to understand how to design and configure a basic network infrastructure in AWS using a Virtual Private Cloud (VPC). This lab focuses on creating a VPC with a public subnet, configuring an Internet Gateway and route table, launching an EC2 instance, and hosting a simple web server that can be accessed over the internet.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity

---

## Tools Used

* AWS Management Console
* Amazon VPC
* Amazon EC2
* Internet Gateway
* Route Table
* Security Groups

---

## Tasks Performed

### Task 1: Create a VPC

Create a new Virtual Private Cloud (VPC) with a private IP address range. The VPC acts as a logically isolated network in AWS where all other resources will be deployed.

Students should create a VPC with an appropriate CIDR block (for example, 10.0.0.0/16) and assign a meaningful name.


### Task 2: Create a Public Subnet

Create a subnet inside the VPC to host public resources. Enable auto-assign public IPv4 so that instances launched in this subnet receive a public IP address.

The subnet should use a smaller CIDR range (for example, 10.0.1.0/24).


### Task 3: Create and Attach Internet Gateway

Create an Internet Gateway (IGW) and attach it to the VPC. This allows communication between resources in the VPC and the internet.


### Task 4: Configure Route Table

Create a route table and add a default route (0.0.0.0/0) pointing to the Internet Gateway. Associate this route table with the public subnet.

This step ensures that traffic from the subnet can reach the internet.


### Task 5: Create Security Group

Create a security group to act as a virtual firewall for the EC2 instance. Configure inbound rules to allow:

SSH on port 22

HTTP on port 80


### Task 6: Launch EC2 Instance

Launch an EC2 instance inside the public subnet using Amazon Linux 2 AMI and a suitable instance type (t2.micro).

Attach the previously created security group and key pair.


### Task 7: Configure Web Server

Install and start a web server (Apache HTTPD) on the EC2 instance using user data or manual commands.

Create a simple HTML page and verify that it can be accessed from a web browser using the public IP address of the instance.---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. First, I created a VPC in Amazon Web Services. I gave it a CIDR block of 10.0.0.0/16. This VPC acts as my private network where all my resources will be created.
2. Next, I created a public subnet inside the VPC with CIDR 10.0.1.0/24. I enabled auto-assign public IP so that any instance launched in this subnet will automatically get a public IP address.
3. After that, I created an Internet Gateway and attached it to my VPC. This allows my VPC to communicate with the internet.
4. Then, I created a route table and added a default route (0.0.0.0/0) pointing to the Internet Gateway. I associated this route table with my public subnet. This step ensures that traffic from my subnet can reach the internet.
5. Next, I created a security group which acts as a virtual firewall. I allowed inbound traffic for SSH on port 22 and HTTP on port 80.



## Output Screenshots (Attach 3)

### Screenshot 1: VPC and Subnet Details

<img width="1254" height="699" alt="image" src="https://github.com/user-attachments/assets/e7d94c2c-56dc-4e75-8d66-cc81b1beec8f" />


---

### Screenshot 2: EC2 Instance Running

<img width="1261" height="561" alt="image" src="https://github.com/user-attachments/assets/20157bdf-3870-41b3-b94e-af5dae2af280" />


---

### Screenshot 3: Web Server Output in Browser

<img width="1267" height="670" alt="image" src="https://github.com/user-attachments/assets/f119ba53-7f13-49ec-8a39-c0b890acb0cd" />


---

## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.
