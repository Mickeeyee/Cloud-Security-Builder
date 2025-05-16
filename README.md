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


---

## 📊 Phase 4: Monitoring and Logging

- Enabled **CloudTrail** to track S3 API events.
- ![image](https://github.com/user-attachments/assets/499fa7c3-e7cd-459b-8712-e91ae18004c4)
- ![image](https://github.com/user-attachments/assets/de559c5d-e4d2-4bb0-8c22-3302efcf449c)
- ![image](https://github.com/user-attachments/assets/831409e1-c5de-4382-9970-0e9d08423b26)
  
- Configured **CloudWatch Agent** and created a **CloudWatch Alarm** to detect SSH brute-force attempts.
- ![image](https://github.com/user-attachments/assets/a98b2d83-033f-4b7c-98a5-48f0067d37c7) ![image](https://github.com/user-attachments/assets/7fc549c4-e8cc-4983-b73c-f2affe4a3a7d)
- ![image](https://github.com/user-attachments/assets/76493cbe-ff91-48b0-b5fa-f4bc900fe224) ![image](https://github.com/user-attachments/assets/005082e9-bf18-4354-acb9-dd31d3f6a048)
- ![image](https://github.com/user-attachments/assets/5272e0f2-5547-4b4b-8ad8-0efd5c960785) ![image](https://github.com/user-attachments/assets/5e0ec493-032e-41fa-929b-4fe7dcbfb357)
- Cloudwatch Alarm
- ![image](https://github.com/user-attachments/assets/329238f9-f3e1-4715-99f1-8ef8b60b422b) ![image](https://github.com/user-attachments/assets/e1fe2044-466f-4e95-9805-41e99977d5dc)
- ![image](https://github.com/user-attachments/assets/794de50c-e9d1-4b16-9204-8c1f588fa765) ![image](https://github.com/user-attachments/assets/9bd3dcd8-7218-48c0-b56a-0e820d92e334)


- Used **AWS Config** to detect and auto-remediate non-compliant S3 bucket logging settings.
- ![image](https://github.com/user-attachments/assets/56e5dc97-7357-46bf-9c34-276bdcbbbe09) ![image](https://github.com/user-attachments/assets/32cc86e9-7514-4158-842f-3b5bc63f395f)
- ![image](https://github.com/user-attachments/assets/831f7984-a1de-4e44-b793-f1893e1d3bfd) ![image](https://github.com/user-attachments/assets/d2c8fee8-d067-40ba-a2c2-c01ef4a0f33a)
- ![image](https://github.com/user-attachments/assets/d64df260-2bc6-4497-9aaa-7d038367aefa) ![image](https://github.com/user-attachments/assets/e2e9dbfb-69f8-43c1-abbd-c2f8373a6c83)
- ![image](https://github.com/user-attachments/assets/92efb417-f837-41b5-8a14-b6b259d3de5d) 








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


