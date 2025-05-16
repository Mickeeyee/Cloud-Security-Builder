# 🔐 AWS Security & Monitoring Lab Project

This project is part of my coursework at George Brown College, where I completed a hands-on lab titled **"Cloud Security Builder: Securing and Monitoring Resources with AWS"**. The lab involved securing, monitoring, and configuring cloud infrastructure using various AWS services.

## 📁 Overview

The lab was divided into four phases, each focusing on different aspects of AWS security, from S3 bucket policies and VPC flow logs to AWS KMS encryption and centralized monitoring using CloudWatch, CloudTrail, and AWS Config.

---

## ✅ Phase 1: Securing Data in Amazon S3

- Created and secured an S3 bucket using bucket policies and tested access with IAM users.
- ![image](https://github.com/user-attachments/assets/14dc4021-ab6a-4e61-a8b6-592270dd261c)
- Enabled versioning and object-level logging.
- ![image](https://github.com/user-attachments/assets/77f2cbc7-65c7-4723-ac37-47f89a5167bb)
-![image](https://github.com/user-attachments/assets/b82fb324-8f49-4a1c-99bc-7d29aaf0f297)
- Implemented S3 Inventory and confirmed versioning functionality.
- Verified object-level logging and queried logs with **Amazon Athena**.
![image](https://github.com/user-attachments/assets/f4562748-347a-4b91-a651-62d46cba6974)
  ![image](https://github.com/user-attachments/assets/f614db07-7b8d-41b1-99a6-35f41eed203a)


---

## 🌐 Phase 2: Securing VPCs

- Reviewed VPC resources and created **VPC Flow Logs**.
- ![image](https://github.com/user-attachments/assets/001725c2-6665-49c2-8a67-9152314b2eaf)
- ![image](https://github.com/user-attachments/assets/fa164ba3-4297-41d8-a49c-523768699139)
- ![image](https://github.com/user-attachments/assets/510a5c44-9c6d-4674-aaed-0d0416970df6)
- 
- Configured **Route Tables**, **Security Groups**, and **Network ACLs** to control traffic.
- ![image](https://github.com/user-attachments/assets/6d9db8a0-be16-4f26-a58e-11276b7c6033)
- ![image](https://github.com/user-attachments/assets/8dd856f8-6a1b-4ea3-a7cd-2559c6190ef4)
- 
- Deployed and configured **AWS Network Firewall** with logging and policy testing.
- Network Firewall created ![image](https://github.com/user-attachments/assets/a2eeddf8-8b8e-485b-a60b-94e9abc63cf8)
- Logging Config ![image](https://github.com/user-attachments/assets/2fc47f54-7da3-4300-8bdf-b7bac295ed0c)
- Policy testing ![image](https://github.com/user-attachments/assets/99c79d40-a0f9-4950-8e91-3d81c6b14862)
- ![image](https://github.com/user-attachments/assets/e70c83f1-4a32-498f-8a9d-526feb30d9d4)


---

## 🔐 Phase 3: Securing AWS Resources Using AWS KMS

- Created Customer Managed Keys with rotation.
- ![image](https://github.com/user-attachments/assets/2926560f-ee37-41ac-8dae-2d73368fcac0)

- Applied AWS KMS policies and tested IAM access.
- ![image](https://github.com/user-attachments/assets/6db4d1bd-a83e-4279-9432-fb2016e4e6b5) The policy allows full control of all S3 buckets within the account and grants the ability to encrypt and decrypt objects. This policy is attached to the FinancialAdvisorGroup IAM group

- Encrypted:
  - S3 data uploads using KMS keys
  - Root volume of an EC2 instance
  - Connect to EC2 ![image](https://github.com/user-attachments/assets/db097d55-c824-48d6-859a-1f06e9c7c893)
  - ![image](https://github.com/user-attachments/assets/48d49ec3-07bc-4e16-b66a-cf957b3a9404) ![image](https://github.com/user-attachments/assets/267e924d-fa83-45a9-97c5-1a7ff76f8481)

  - Secrets in AWS Secrets Manager
  - ![image](https://github.com/user-attachments/assets/004c8cdb-c602-4605-a909-52f19849963d) ![image](https://github.com/user-attachments/assets/378b6367-c9a2-4317-814d-8774a5406b61)
  - ![image](https://github.com/user-attachments/assets/b3ed06dd-534e-495a-9cf6-a47721b8b2d7) ![image](https://github.com/user-attachments/assets/a829f389-45ac-4c95-93d9-5e7381a0bf5a)

- Implemented envelope encryption with KMS for local files.

---

## 📊 Phase 4: Monitoring and Logging

- Enabled **CloudTrail** to track S3 API events.
- Configured **CloudWatch Agent** and created a **CloudWatch Alarm** to detect SSH brute-force attempts.
- Used **AWS Config** to detect and auto-remediate non-compliant S3 bucket logging settings.

---

## 💡 Tools & Services Used

- Amazon S3
- Amazon VPC, EC2, Route Tables, Security Groups, NACLs
- AWS Network Firewall
- AWS KMS
- AWS Secrets Manager
- AWS CloudTrail
- Amazon Athena
- Amazon CloudWatch & Alarms
- AWS Config

---

## 🧠 Key Learnings

- Applied **least privilege principles** using IAM and KMS policies.
- Gained practical experience in **infrastructure security**, **log monitoring**, and **automated compliance**.
- Developed a deeper understanding of how to **secure cloud environments end-to-end**.

---


