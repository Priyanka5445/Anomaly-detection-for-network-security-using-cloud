# Anomaly Detection for Network Security Using Cloud

Real-time ML system to detect network threats — DDoS, Port Scanning, 
and Brute Force attacks — using cloud infrastructure on AWS and Azure.

## Project Overview
Built and deployed a cloud-native machine learning pipeline that 
classifies malicious network activity from simulated traffic logs. 
Integrated AWS SageMaker for model training and Azure Monitor for 
deployment and monitoring.

## Dataset
- 10,001 network traffic log records
- 14 features including: packet rate, packet size, protocol, 
  authentication success, request count, unique source IPs, 
  token metadata, and attack type labels
- Attack categories: DDoS, Port Scanning, Brute Force

## Models Evaluated
| Model  | Accuracy | Precision | Recall | F1-Score |
|--------|----------|-----------|--------|----------|
| SVM    | 66.67%   | 66.67%    | 66.67% | 66.67%   |
| KNN    | —        | —         | —      | —        |
| Hybrid | 66.67%   | 66.67%    | 66.67% | 66.67%   |

> Note: Results reflect class imbalance in the dataset. 
> SMOTE-based resampling and tuning is planned as next iteration.

## Tech Stack
- Python, Scikit-learn, Pandas, NumPy
- AWS SageMaker, Azure Monitor
- Power BI (threat visualization dashboards)
- Git, GitHub, VS Code

## Project Structure
- Dataset/ — raw and processed network traffic data
- models/ — trained ML model files
- cloud dataset.csv — full feature dataset (10,001 records)
- features.csv — feature definitions
- metrics.json — model evaluation results
- preprocessed.csv — cleaned and encoded dataset
- Requirements.txt — Python dependencies
- runserver.bat — local server launcher

## How to Run
1. Install dependencies:
pip install -r Requirements.txt
2. Launch the server:
Double-click runserver.bat
