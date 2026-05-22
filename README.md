Serverless Employee Management Web Application
📌 Project Overview
This project is a fully serverless employee management web application built on AWS Cloud.
The application allows users to insert and retrieve employee data using REST APIs integrated with AWS Lambda and DynamoDB.
The frontend is securely hosted in a private Amazon S3 bucket and delivered globally using Amazon CloudFront with HTTPS enabled through AWS Certificate Manager (ACM) and custom domain integration.

🚀 Live Demo
https://serverless.cloudbimal.in

🏗️ Architecture
User → Route53 → CloudFront → Private S3 Bucket → API Gateway → Lambda → DynamoDB

☁️ AWS Services Used
Service	Purpose
Amazon S3	Frontend hosting
Amazon CloudFront	CDN & secure delivery
AWS Certificate Manager (ACM)	SSL/TLS certificate
Amazon Route53	Custom domain DNS
AWS Lambda	Backend serverless compute
Amazon API Gateway	REST API management
Amazon DynamoDB	NoSQL database
IAM Roles & Policies	Secure permissions
CloudFront OAC	Secure private S3 access

✨ Features
Fully serverless architecture 
Employee data insertion 
Retrieve employee records 
REST API integration 
HTTPS secured website 
Custom domain support 
Private S3 bucket security 
Scalable and cost-effective design 

📂 Project Structure
project/
│
├── frontend/
│   ├── index.html
│   └── scripts.js
│
├── lambda/
│   ├── insertEmployeeData.py
│   └── getEmployees.py
│
├── screenshots/
│
├── architecture.png
│
└── README.md

🔧 Deployment Steps
1️⃣ Create DynamoDB Table
Table Name: employeeData 
Partition Key: employeeid 

2️⃣ Create Lambda Functions
insertEmployeeData 
getEmployees 
Attach IAM Role with DynamoDB permissions.

3️⃣ Configure API Gateway
Create REST API 
Configure GET and POST methods 
Enable CORS 
Deploy API stage 

4️⃣ Upload Frontend to S3
Create private S3 bucket 
Upload: 
oindex.html 
oscripts.js 

5️⃣ Configure CloudFront
Create distribution 
Use S3 bucket as origin 
Configure Origin Access Control (OAC) 
Set: 
oDefault root object = index.html 

6️⃣ Configure HTTPS
Request SSL certificate using ACM 
Validate domain ownership 

7️⃣ Configure Route53
Create hosted zone 
Point domain to CloudFront distribution 

🔒 Security Implementation
Private S3 bucket 
CloudFront OAC enabled 
HTTPS/TLS enabled 
IAM least privilege permissions 
API CORS configured 
 

📈 Future Improvements
CI/CD Pipeline using GitHub Actions or Jenkins 
Terraform Infrastructure as Code 
Docker containerization 
Monitoring with CloudWatch 
Authentication using Cognito 

👨‍💻 Author
Bimal Kumar Maharana
AWS Cloud & DevOps Enthusiast 
MCA Graduate 
Skilled in AWS, Python, Linux, DevOps & Data Analytics 

📬 Contact
LinkedIn: Add your LinkedIn profile here
GitHub: Add your GitHub repository link here
