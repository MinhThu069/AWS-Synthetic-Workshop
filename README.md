# AWS Synthetic Data Generation Workshop

[![AWS](https://img.shields.io/badge/AWS-S3-orange.svg)](https://aws.amazon.com/s3/)
[![AWS](https://img.shields.io/badge/AWS-Glue-yellow.svg)](https://aws.amazon.com/glue/)
[![AWS](https://img.shields.io/badge/AWS-Macie-blue.svg)](https://aws.amazon.com/macie/)
[![AWS](https://img.shields.io/badge/AWS-SageMaker-purple.svg)](https://aws.amazon.com/sagemaker/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A hands-on workshop to help you **build a Synthetic Data Generation Platform with Privacy Preservation** using AWS.  
Learn how to upload, preprocess, anonymize, and generate high-quality synthetic datasets — ensuring privacy, compliance, and reusability.

---

## 🧠 Problem Background

In many organizations, especially in **banking and finance**, real datasets contain sensitive or personally identifiable information (PII).  
Sharing or using such data can lead to privacy breaches, compliance violations, and slow collaboration between teams.  
Manual anonymization is often:
- **Time-consuming** and error-prone
- **Risky** due to potential PII leaks
- **Limiting** collaboration between technical and business teams
- **Slowing down** AI/ML research and development

This workshop addresses these issues by building an **automated, privacy-preserving synthetic data generation pipeline** on AWS.

---

## 🏗️ Architecture Overview

```plaintext
CSV Dataset
    ↓
Amazon S3
    ↓
AWS Glue (Data Preprocessing)
    ↓
Amazon Macie (PII Detection & Removal)
    ↓
SageMaker Studio Lab (TVAE Model)
    ↓
Synthetic Data Output
    ↓
Statistical Evaluation & Visualization
```

🎯 Learning Objectives
After completing this workshop, you will be able to:
✅ Upload datasets to Amazon S3
✅ Preprocess and normalize schema with AWS Glue
✅ Detect and remove PII with Amazon Macie
✅ Train a TVAE model in SageMaker Studio Lab to generate synthetic data
✅ Evaluate the similarity between synthetic and original datasets

📁 Workshop Folder Structure
| Path                      | Description                                        |
| ------------------------- | -------------------------------------------------- |
| `1_upload_to_s3/`         | Upload raw CSV data to Amazon S3                   |
| `2_data_cleaning/`        | Data preprocessing and schema normalization (Glue) |
| `3_pii_detection/`        | PII scanning and removal with Amazon Macie         |
| `4_synthetic_generation/` | Train TVAE model and generate synthetic dataset    |
| `5_evaluation/`           | Compare statistical distributions & correlations   |
| `6_report/`               | Diagrams, screenshots, deployment evidence         |
| `7_conclusion/`           | Summary of results and key learnings               |



🛠️ AWS Services Used

- Amazon S3: Store raw and synthetic datasets
- AWS Glue: Data cleaning and transformation
- Amazon Macie: PII detection and reporting
- Amazon SageMaker Studio Lab: Train synthetic data generation model (TVAE)
- IAM: Secure access and role management

💻 Prerequisites
✅ AWS account with permissions for:
- Amazon S3
- AWS Glue
- Amazon Macie
✅ AWS account with SageMaker permissions
✅ Python 3.8+ with boto3, sagemaker, pandas
✅ Basic knowledge of Jupyter Notebook or script execution


🌟 Key Benefits
✅ Business Benefits
- Safe sharing of datasets without privacy risk
- Faster AI/ML project delivery
- Reduced compliance overhead

🔧 Technical Improvements
- Automated PII detection and removal
- Reproducible synthetic data pipelines
- Consistent schema validation and distribution checks

🔭 Long-Term Vision
- Real-time synthetic data streaming
- Integration with enterprise MLOps pipelines
- Multi-table relational dataset generation

💰 Cost Estimation
This workshop was designed to run within AWS Free Tier:
| Service              | Estimated Cost | Notes                             |
| -------------------- | -------------- | --------------------------------- |
| Amazon S3            | \~\$0          | Free Tier 5GB storage             |
| AWS Glue             | \~\$0–1        | Small datasets only               |
| Amazon Macie         | \~\$0–1        | Low scanning cost for sample data |
| SageMaker Studio Lab | Free           | Community resources               |
| Total                | **< \$3 USD**  | Under normal usage limits         |


📚 Workshop Steps

- Upload Data to Amazon S3
- Preprocess Data with AWS Glue
- Detect & Remove PII with Amazon Macie
- Train TVAE Model to Generate Synthetic Data
- Evaluate Statistical Similarity & Privacy
- Document and Report Findings
- Conclusion and Recommendations

🔐 Best Practices Implemented
🔒 Least Privilege IAM Roles
🔄 Reusable data generation pipeline
📦 Schema consistency checks between raw & synthetic data
📊 Statistical quality validation before usage

🚀 Quick Start (Local)
```bash
git clone https://github.com/MinhThu069/aws-synthetic-workshop.git
cd aws-synthetic-workshop
pip install -r requirements.txt
```
You can run the scripts in order or explore each notebook in .ipynb format.

🤝 Contributing
- Pull requests are welcome. For major changes, please open an issue first.

📄 License
- This project is licensed under the MIT License. See LICENSE for details.

📬 Contact & Feedback
📧 Email: nguyenthiminhthu92003@gmail.com
🐛 Issues: GitHub Issues