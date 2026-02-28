# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: Yasvanth D
* **Register Number**: 212223090031
* **Date of Submission**: 28/02/26

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1.Created an Amazon EBS volume

2.Attached the volume to an EC2 instance

3.Created a file system on the volume

4.Added a file to volume

5.Created a snapshot of volume

6.Created a new volume from the snapshot

7.Attached and mounted the new volume to the EC2 instance

8.Verified that the file created earlier was on the newly created volume

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1650" height="774" alt="image" src="https://github.com/user-attachments/assets/c77ee26a-7cdd-444c-b477-9333e23bfde4" />
<img width="1639" height="754" alt="image" src="https://github.com/user-attachments/assets/fa8cc064-a8af-461b-aa27-1b24fa183f5d" />



---

### Screenshot 2: EBS Volume Attached to EC2
<img width="1588" height="501" alt="image" src="https://github.com/user-attachments/assets/a9a5b524-3b79-4130-9c00-7c71724a539d" />
<img width="1622" height="698" alt="image" src="https://github.com/user-attachments/assets/513dfa37-9c08-489d-bb90-4538489b8fa1" />



---

### Screenshot 3: Mounted Volume with Data

<img width="1642" height="820" alt="image" src="https://github.com/user-attachments/assets/ccd6df88-32bf-4a8d-9bbb-c42d18011487" />
<img width="1619" height="860" alt="image" src="https://github.com/user-attachments/assets/19784a9f-2184-4627-97a3-6466ba980688" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
