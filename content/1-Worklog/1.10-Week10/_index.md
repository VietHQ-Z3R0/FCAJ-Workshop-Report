---
title: "Week 10 Worklog"
date: 2026-11-07
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

# **Week 10 Work Log: ReLoop AWS Architecture Review & Service Integration Validation**

## **1. Weekly Objectives**

* Review the overall ReLoop AWS architecture.
* Verify service communication flows and architectural boundaries.
* Examine authentication, storage, backend and AI integration.
* Improve the accuracy and clarity of AWS architecture documentation.

## **2. Weekly Execution Schedule**

| Day | Task Description | Start Date | Completion Date | Reference Material |
| :--- | :--- | :--- | :--- | :--- |
| **Day 1** | Started reviewing the ReLoop AWS architecture diagram and identifying its main service interactions | 11/16/2026 | 11/16/2026 | [Modernize Applications on AWS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Day 2** | Reviewed CloudFront origins, S3 Origin Access Control and API Gateway request routing | 11/17/2026 | 11/17/2026 | [CloudFront Origin Access Control](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html) |
| **Day 3** | Examined Cognito authentication, JWT authorization and Lambda user profile triggers | 11/18/2026 | 11/18/2026 | [API Gateway JWT Authorizer](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-jwt-authorizer.html) |
| **Day 4** | Reviewed S3 Presigned URL workflows, DynamoDB data access and AI service integration | 11/19/2026 | 11/19/2026 | [S3 Presigned URLs](https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-presigned-url.html) |
| **Day 5** | Refined the architecture diagram and reviewed EventBridge, AI processing and monitoring connections | 11/20/2026 | 11/20/2026 | [Kimi K3 – Amazon Bedrock](https://docs.aws.amazon.com/bedrock/latest/userguide/model-card-moonshot-ai-kimi-k3.html) |

## **3. Key Achievements & Outcomes**

### **Architecture Understanding**

* Started a detailed review of the ReLoop architecture on 16/11/2026.
* Improved understanding of the relationship between CloudFront, API Gateway and backend services.
* Reviewed the authentication workflow involving Amazon Cognito and JWT authorization.
* Examined the separation between static website storage and device image storage.

### **Technical Analysis**

* Reviewed the Presigned URL mechanism for direct browser-to-S3 image uploads and downloads.
* Examined DynamoDB read and write operations in the backend architecture.
* Reviewed the responsibilities of Amazon Rekognition in image moderation and text detection.
* Researched Amazon Bedrock Kimi K3 and Guardrails for AI-assisted image analysis.
* Reviewed EventBridge scheduling and CloudWatch monitoring flows.

### **Documentation & Deliverables**

* Refined the ReLoop AWS architecture diagram and improved labeling and direction of service communication flows.
* Identified unclear architectural relationships requiring additional verification and organized updated architecture information for the final project documentation.
