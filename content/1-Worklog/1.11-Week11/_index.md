---
title: "Week 11 Worklog"
date: 2026-11-23
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

# **Week 11 Work Log: Final Integration Validation, Report Submission & Expansion Research**

## **1. Weekly Objectives**

* Complete final end-to-end integration checks across the ReLoop AWS environment.
* Clean up unused assets/resources and verify observed AWS costs against remaining credits.
* Finalize and submit the complete internship report and ReLoop project documentation (24–25/11/2026).
* Research potential architectural extensions and AWS security enhancements for future iterations of ReLoop.

## **2. Weekly Execution Schedule**

| Day | Task Description | Start Date | Completion Date | Reference Material |
| :--- | :--- | :--- | :--- | :--- |
| **Day 1** | Completed final integration validation (S3 Presigned URLs, Rekognition + Bedrock Guardrail moderation, Kimi K3 listing flow) and cleaned up unused static assets and AWS resources | 11/23/2026 | 11/23/2026 | [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) |
| **Day 2** | Consolidated the final AWS architecture diagram (`draw.io` + PNG), verified AWS Billing/Credits, and completed proofreading across Worklog, Proposal, Blogs, Events, Workshop, Self-Evaluation & Feedback | 11/24/2026 | 11/24/2026 | [FCJ Workforce Program](https://cloudjourney.awsstudygroup.com/8-fcjworkforce/) |
| **Day 3** | Submitted the finalized internship report and ReLoop technical documentation package via GitHub Pages | 11/25/2026 | 11/25/2026 | [The First Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **Day 4** | Researched future expansion options for ReLoop, including migrating Cognito email delivery to Amazon SES (beyond the 50 emails/day default limit) and real-time chat via API Gateway WebSockets | 11/26/2026 | 11/26/2026 | [Amazon SES Developer Guide](https://docs.aws.amazon.com/ses/latest/dg/Welcome.html) |
| **Day 5** | Explored Shift-Left IaC security scanning for Terraform in GitHub Actions and reviewed CloudWatch Logs, alarms, and WAF metrics on the live deployment | 11/27/2026 | 11/27/2026 | [Amazon CloudWatch Alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Alarms.html) |

## **3. Key Achievements & Outcomes**

### **Final Validation & Resource Hygiene**

* Verified all 10 architecture flows across CloudFront, WAF, Cognito, API Gateway, Lambda, DynamoDB, S3, Rekognition, and Bedrock Kimi K3.
* Audited and cleaned up unused repository assets and checked AWS spend against remaining credits.

### **Internship Report & Documentation Submission**

* Completed and published the full bilingual (EN/VI) internship report—including the 12-week Worklog, Proposal, 3 AWS technical blogs, 5 event recaps, 12-module Workshop, Self-Evaluation, and Feedback—by 24–25/11/2026.

### **Future Expansion Research**

* Documented practical next-step improvements for ReLoop: custom Amazon SES email sender, WebSocket-based real-time chat replacing 5-second polling, and automated Terraform security checks in CI/CD.
