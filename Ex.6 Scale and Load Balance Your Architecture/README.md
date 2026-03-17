# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
## NAME: D.Yasvanth (212223090031)

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1.Review Existing Architecture – Examine the previously created Amazon EC2 application setup and understand how the current infrastructure works.
2.Create Launch Template – Configure a launch template specifying the AMI, instance type, security group, and user data for EC2 instances.
3.Set Up Auto Scaling Group – Create an Auto Scaling Group using the launch template and define the minimum, maximum, and desired instance capacity.
4.Configure Application Load Balancer – Set up an AWS Application Load Balancer and create target groups to distribute incoming traffic across EC2 instances.
5.Attach and Test Scaling – Connect the Auto Scaling Group to the load balancer target group, configure CPU-based scaling policies using Amazon CloudWatch, and test by generating traffic to observe load balancing and automatic scaling.

---

## Output Screenshots 

<img width="1917" height="1198" alt="image" src="https://github.com/user-attachments/assets/e1118e31-538d-4661-9c16-dc4b94425d04" />

<img width="1917" height="1199" alt="image" src="https://github.com/user-attachments/assets/c827b697-3428-4cd4-9844-9f93d126cf89" />

<img width="1918" height="1199" alt="image" src="https://github.com/user-attachments/assets/83f8829b-7658-4dc7-932d-407eeabbcca5" />

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/471149d8-5dc4-443a-a7e4-47cd0c1eef42" />




---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
