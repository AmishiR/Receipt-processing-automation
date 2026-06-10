# Automated AWS Document Processing System

## Overview of Project ☁️

This project focuses on automating document processing using AWS services. Instead of manually reviewing and managing uploaded documents, the system automatically extracts relevant information, stores the processed data, and generates notifications for users. This approach improves efficiency, reduces manual effort, and enables scalable document management.

The architecture consists of:

* **Storage Layer:** Amazon S3 stores uploaded documents, images, or PDFs.
* **Processing Layer:** Amazon Textract extracts text and key information using AI-powered OCR.
* **Database Layer:** Amazon DynamoDB stores extracted data in a structured format.
* **Notification Layer:** Amazon SES sends email notifications with processing results.
* **Compute Layer:** AWS Lambda orchestrates and automates the workflow in real time.

---

## Services Used 🛠️

* **Amazon S3** – Stores uploaded files and documents. *(Storage)*
* **Amazon Textract** – Extracts text and structured information from documents.
* **Amazon DynamoDB** – Stores processed data for future retrieval.
* **Amazon SES** – Sends automated email notifications.
* **AWS Lambda** – Executes processing logic without managing servers.
* **IAM Roles & Policies** – Provides secure access between AWS services.

---

## Architectural Diagram ✍️

*(Insert architecture diagram here)*

---

## Workflow 🚀

1. User uploads a document to an S3 bucket.
2. S3 triggers an AWS Lambda function.
3. Lambda invokes Amazon Textract to analyze the document.
4. Extracted information is processed and stored in DynamoDB.
5. Amazon SES sends a notification containing the extracted details.
6. The processed data is available for retrieval and auditing.

---

## Project Features ✨

* Automated document ingestion and processing
* AI-powered text extraction using Amazon Textract
* Serverless architecture with AWS Lambda
* Structured data storage in DynamoDB
* Email notifications through Amazon SES
* Scalable and cost-efficient cloud solution

---

## Limitation ⚠️

Amazon Textract usage is limited by AWS pricing policies. The free tier covers only 1,000 pages per month for the first 3 months, after which standard API charges apply. This introduces recurring costs for large-scale or long-term use of the project. Cost monitoring and billing alerts are recommended.

---

## Steps to Perform ☁️

In this project, the following steps are performed:

### 1. Storage Setup

* Create an Amazon S3 bucket
* Configure upload permissions

### 2. Database Setup

* Create a DynamoDB table
* Define partition keys and attributes

### 3. Notification Setup

* Configure Amazon SES
* Verify sender and recipient email addresses

### 4. Processing Setup

* Create and deploy an AWS Lambda function
* Configure IAM permissions

### 5. Integration and Testing

* Connect S3, Lambda, Textract, DynamoDB, and SES
* Upload sample documents and verify results
  


---

## Clean Up 🗑️

To avoid unnecessary AWS charges:

* Delete the S3 bucket and uploaded files
* Delete the DynamoDB table
* Remove Lambda functions
* Disable SES notifications
* Delete IAM roles and policies
* Stop all Textract-related processing

---

## Technologies Used 💻

* Python
* AWS Lambda
* Amazon S3
* Amazon Textract
* Amazon DynamoDB
* Amazon SES
* IAM

---

## Outcome 🎯

The project demonstrates how AWS serverless services can be integrated to build an automated document-processing pipeline that is scalable, efficient, and suitable for real-world business workflows.
