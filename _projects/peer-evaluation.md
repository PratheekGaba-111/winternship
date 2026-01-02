---
layout: project
title: Peer Evaluation
order: 4
summary: Multi-level peer assessment system with automated anomaly detection and escalation workflow
---


## Project Overview

Peer Evaluation is an intelligent assessment management system that facilitates peer-to-peer evaluation of quizzes and assessments with built-in quality control mechanisms. The system assigns unique IDs to each student for every quiz/assessment, ensuring anonymity and security. QR codes are generated from these unique IDs only when teachers use the bulk download option for later uploading bulk PDFs. When students upload their quizzes directly from their portal, unique IDs are generated automatically without QR codes. The system features a sophisticated multi-level review workflow where anomalies detected by algorithm-based analysis are automatically flagged to Teaching Assistants (TAs), who can escalate unresolved issues to teachers, maintaining academic integrity throughout the evaluation process.

## Key Features

- **Unique ID System**: Automatic unique ID generation for each student per quiz/assessment
- **Dual Submission Methods**:
  - **Bulk Download**: Teacher downloads unique IDs with QR codes for offline distribution and bulk PDF upload
  - **Student Portal Upload**: Students upload directly via portal with auto-generated unique IDs (no QR codes needed)
- **Peer Review System**: Students evaluate their peers' work anonymously
- **Algorithm-Based Anomaly Detection**: Automated detection of suspicious patterns, inconsistencies, and outliers
- **Multi-Level Escalation Workflow**: 
  - Student peer reviews → System anomaly detection → TA review → Teacher intervention
- **TA Dashboard**: Interface for TAs to review flagged submissions and resolve issues
- **Teacher Portal**: Final escalation point for complex cases requiring instructor attention
- **Rubric-Based Evaluation**: Standardized criteria for consistent assessment
- **Analytics and Reporting**: Comprehensive insights on evaluation patterns and quality
- **Feedback Management**: Structured peer feedback with quality controls
- **Rating Aggregation**: Statistical analysis to ensure fair final grades
- **Audit Trail**: Complete tracking of evaluation and escalation history

## Technologies Used

- Frontend: React, Javascript
- Backend: Express.js, Node.js
- Database: MongoDB
- QR Code Generation: QR code libraries
- Anomaly Detection: Statistical outlier detection algorithms (Standard Deviation, etc.)
- Authentication: JWT/OAuth

## Evaluation Workflow

### Submission Path 1: Bulk Download (with QR Codes)
1. **Assessment Creation**: Teacher creates quiz/assessment with evaluation rubrics
2. **Bulk Download**: Teacher downloads unique IDs with QR codes for each student
3. **Offline Distribution**: Students receive printed assessments with QR codes
4. **Bulk Upload**: Teacher uploads scanned PDFs linked to QR codes
5. **Peer Evaluation**: Students anonymously evaluate assigned peer submissions

### Submission Path 2: Student Portal Upload (without QR Codes)
1. **Assessment Creation**: Teacher creates quiz/assessment with evaluation rubrics
2. **Student Upload**: Students upload their quiz directly from their portal
3. **Auto ID Generation**: System automatically generates unique IDs (no QR codes)
4. **Peer Evaluation**: Students anonymously evaluate assigned peer submissions

### Common Workflow (Both Paths)
5. **Algorithm-Based Analysis**: System analyzes evaluations for anomalies (bias, inconsistencies, outliers)
6. **TA Review**: Flagged cases are sent to TAs for investigation
7. **Teacher Escalation**: Unresolved cases are escalated to teachers for final decision
8. **Marks Finalization**: Validated evaluations are aggregated for final marks

## Project Goals

1. Implement fair and transparent multi-level evaluation system
2. Ensure anonymity through unique ID-based identification
3. Support flexible submission methods (bulk upload with QR codes or student portal)
4. Automate detection of evaluation anomalies using robust algorithms
5. Create efficient escalation workflow (Peers → System → TAs → Teachers)
6. Generate comprehensive analytics on evaluation quality
7. Maintain academic integrity throughout the assessment process
8. Provide actionable insights for continuous improvement

## GitHub Repository

[PES](https://github.com/vicharanashala/pes)
