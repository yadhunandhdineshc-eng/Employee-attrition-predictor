

# Employee Attrition Predictor

![Python](https://img.shields.io/badge/Python-Flask-blue)
![React](https://img.shields.io/badge/Frontend-React-blue)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning--green)

## 📌 Project Overview

Employee Attrition Predictor is a web-based machine learning application designed to predict the probability of employee attrition based on various HR and workplace-related factors.

The system analyzes employee information such as job satisfaction, salary, work experience, overtime, work-life balance, and other HR metrics to predict whether an employee is at risk of leaving the organization.

The application also provides dashboards, analytics, role-based access control, data upload functionality, job vacancy management, and job application tracking.

---

## 🎯 Objective

The main objective of this project is to help organizations:

- Predict employee attrition
- Identify employees with a higher risk of leaving
- Analyze employee attrition trends
- Support HR teams with data-driven insights
- Improve employee retention strategies
- Reduce recruitment and replacement costs

---

## ✨ Features

### 🤖 Employee Attrition Prediction

The application predicts:

- Employee attrition outcome
- Attrition risk percentage
- Risk level

Risk levels are classified as:

- 🟢 Low Risk
- 🟡 Medium Risk
- 🔴 High Risk

---

### 📊 Analytics Dashboard

The dashboard provides insights such as:

- Total employees
- Employee attrition rate
- Employee retention rate
- Department-wise attrition
- Attrition trends
- Retention analysis

---

### 👥 Role-Based Access Control

The system supports multiple user roles:

#### 🔐 Admin

- Manage users
- Approve or reject user registrations
- View dashboards and reports
- Upload employee datasets
- Predict employee attrition
- View job applications

#### 👨‍💼 HR Manager

- View HR reports
- Upload employee datasets
- Predict employee attrition

#### 📊 Data Analyst

- View attrition trends
- Analyze department-wise attrition
- Access charts and visualizations
- Upload employee datasets
- Predict employee attrition

#### 👨‍💻 Employee

- Register and log in after admin approval
- View job vacancies
- Apply for jobs
- Upload resumes
- Track job applications
- Predict employee attrition risk

#### 👤 User

- Register and log in after admin approval
- View available job vacancies
- Apply for jobs
- Upload resumes
- Track job application status

---

## 📤 Data Upload

The application allows authorized users to upload employee datasets.

Supported formats:

- CSV
- XLS
- XLSX

After uploading a dataset, the application validates the file and provides a preview of the uploaded data.

---

## 🧠 Machine Learning

The machine learning model analyzes multiple employee-related features, including:

- Age
- Business travel
- Daily rate
- Distance from home
- Education
- Education field
- Environment satisfaction
- Gender
- Job involvement
- Job level
- Job role
- Job satisfaction
- Marital status
- Monthly income
- Number of companies worked
- Overtime
- Salary hike
- Performance rating
- Relationship satisfaction
- Stock options
- Total working years
- Work-life balance
- Years at company
- Years in current role
- Years since last promotion
- Years with current manager

The system returns an employee attrition prediction along with a risk percentage and risk level.

---

## 🛠️ Technology Stack

### Frontend

- React.js
- JavaScript
- HTML
- CSS

### Backend

- Python
- Flask

### Database

- MySQL

### Machine Learning

- Scikit-learn

### Data Visualization

- Matplotlib
- Seaborn
- Plotly

### Authentication

- JWT (JSON Web Token)


---


## 📄 Disclaimer

This project was developed for academic and educational purposes. Any datasets or employee information used for testing should be handled responsibly and in accordance with applicable data protection and privacy regulations.

👉 [View the Detailed Project Report] (

---


## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │     React Frontend   │
                    │                     │
                    │ Dashboards          │
                    │ Prediction          │
                    │ User Management     │
                    │ Job Applications    │
                    └──────────┬──────────┘
                               │
                               │ HTTP / REST API
                               ▼
                    ┌─────────────────────┐
                    │    Flask Backend    │
                    │                     │
                    │ Authentication      │
                    │ RBAC                │
                    │ Prediction API      │
                    │ Dashboard API       │
                    │ Job Management      │
                    └───────┬─────┬───────┘
                            │     │
                            ▼     ▼
                   ┌───────────┐ ┌──────────────┐
                   │   MySQL   │ │ ML Model     │
                   │ Database  │ │ Scikit-learn │
                   └───────────┘ └──────────────┘


