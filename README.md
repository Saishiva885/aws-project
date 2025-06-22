# 📧 Serverless Email Sender using AWS Lambda & SES

This is a simple serverless email automation project built using **AWS Lambda**, **Amazon SES**, and **API Gateway**. It sends a professionally formatted HTML email when triggered via an HTTP request.

The project was developed for **SR Constructions** as part of my AWS Cloud learning journey.

---

## 🔧 What This Project Does

- Sends a welcome email through **Amazon SES**
- Triggered by an HTTP POST request to **API Gateway**
- Backend logic written in **Python using AWS Lambda**
- Email delivery tested from an **EC2 instance** using `curl`
- Logging and debugging handled with **CloudWatch**

---

## 🛠️ Technologies Used

- AWS Lambda (Python 3.12)
- Amazon SES (Simple Email Service)
- Amazon API Gateway (HTTP API)
- AWS CloudWatch (Log Monitoring)
- IAM (Role-based access)
- EC2 (for endpoint testing)
- boto3 (AWS SDK for Python)

---

## ✉️ Email Preview

- **From**: `thatiparthisaishiva@gmail.com` *(verified in SES)*
- **To**: `thatiparthisaikrishna@gmail.com` 
- **Subject**: `Welcome to SR Constructions`
- **Body**: Professionally styled HTML email with header, body, and footer

---

## 💻 How I Tested the Project

1. Created and deployed Lambda function with Python code
2. Verified my sender email in **Amazon SES**
3. Created an **API Gateway POST endpoint** and connected it to Lambda
4. Launched an EC2 instance for testing
5. Ran the following `curl` command:

```bash
curl -X POST https://<your-api-id>.execute-api.us-east-1.amazonaws.com/send-email
