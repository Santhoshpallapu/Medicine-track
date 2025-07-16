# AWS MedTrack

A medical appointment tracking system built with Flask and AWS services.

## Features

- Patient registration and login
- Appointment booking system
- Doctor and patient dashboards
- Profile management
- AWS integration for storage and services

## AWS Deployment Requirements

### Prerequisites
- AWS Account with necessary permissions
- AWS CLI installed and configured
- IAM roles with appropriate permissions

### Required AWS Services
1. EC2 Instance (t2.micro recommended)
2. Elastic Load Balancer (Application Load Balancer)
3. RDS PostgreSQL Database
4. S3 Bucket for static assets
5. Security Groups
6. IAM Roles and Policies

### Security Considerations
- Proper security group rules
- SSL/TLS certificates
- Regular security patches
- Database encryption
- Environment variable management

## Local Setup Instructions

1. Create a virtual environment:
```bash
python -m venv .venv
```

2. Activate the virtual environment:
```bash
.venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables in .env file

5. Run the application:
```bash
python app.py
```

## AWS Deployment Instructions

1. Create AWS resources using CloudFormation or AWS Console
2. Configure security groups and network settings
3. Deploy code using AWS CodeDeploy or EB CLI
4. Set up environment variables in AWS Elastic Beanstalk
5. Configure SSL/TLS certificates
6. Set up monitoring and logging

## Project Structure

```
awsmedtrack-main/
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── deploy.json         # AWS deployment configuration
├── README.md          # Project documentation
├── .env               # Environment variables
├── app.log            # Application logs
├── static/            # Static assets (CSS, JS, images)
│   └── style.css
└── template/          # HTML templates
    ├── base.html
    ├── book_appointment.html
    ├── doctor_dashboard.html
    ├── index.html
    ├── login.html
    ├── patient_dashboard.html
    ├── profile.html
    └── register.html
    └── view_appointment.html
```
