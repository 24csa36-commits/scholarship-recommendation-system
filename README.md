# scholarship-recommendation-system
📌 Project Overview

The AI-Based Scholarship Recommendation System is a full-stack web application designed to simplify the scholarship discovery process for students across India.

The system collects student profile details and intelligently filters All India, State Government, and Private scholarships based on eligibility conditions such as:

Category (SC/ST/OBC/General)

Annual Family Income

Academic Percentage

Gender

State

Course Level (UG/PG/PhD)

Special Categories (PWD, Minority, etc.)

The goal of this project is to improve awareness, accessibility, and transparency in scholarship applications.

🚀 Key Features
👤 Student Module

Student Registration & Login

Profile Creation

Smart Eligibility Matching

Scholarship Recommendation List

Deadline Notifications

Save/Bookmark Scholarships

🛠 Admin Module

Add / Edit / Delete Scholarships

Manage Eligibility Criteria

Update Deadlines

Monitor Student Usage

📊 Analytics Module

Scholarship distribution statistics

Category-wise filtering

Income-based eligibility analysis

Dashboard charts using Chart.js

🏗 System Architecture
Frontend (HTML + CSS + Bootstrap)
        ↓
Flask Backend (Python)
        ↓
Eligibility Engine (Filtering Logic)
        ↓
Database (SQLite / MySQL)
🧠 Eligibility Matching Logic

The system compares:

Student Profile Data
with
Scholarship Eligibility Criteria

It calculates matching conditions and returns only eligible scholarships.

Example Logic:

If Income ≤ Scholarship Income Limit

If Category matches

If Percentage ≥ Minimum Requirement

If State matches (or All India)

Then → Scholarship is recommended.

🛠 Tech Stack
💻 Frontend

HTML5

CSS3

Bootstrap 5

JavaScript

Chart.js

⚙ Backend

Python

Flask Framework

🗄 Database

SQLite (Development)

MySQL (Production Ready Option)

🔧 Tools

Git & GitHub

VS Code

Postman (API Testing)

Trello (Project Management)

📂 Project Structure
scholarship-recommendation-system/
│
├── app/
│   ├── __init__.py
│   ├── routes.py
│   ├── models.py
│   ├── eligibility.py
│   ├── templates/
│   ├── static/
│
├── database/
│   ├── schema.sql
│
├── requirements.txt
├── config.py
├── run.py
├── README.md
👥 Team Structure
Role	Responsibility
Backend Developer	Flask setup, API, eligibility logic
Frontend Developer	UI design, responsive layout
Database Engineer	Schema design, data collection
Analytics Developer	Dashboard charts & reports
Project Lead	Architecture design & Git workflow
🔄 Git Workflow Strategy

We follow a branch-based development model.

main → Stable Production Code

dev → Development Branch

feature-branch-name → Individual Features

Example:

git checkout -b login-feature
git add .
git commit -m "Implemented login system"
git push origin login-feature

Then create a Pull Request → Merge to dev.

⚙ Installation Guide
1️⃣ Clone Repository
git clone https://github.com/your-username/scholarship-recommendation-system.git
cd scholarship-recommendation-system
2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate   (Mac/Linux)
venv\Scripts\activate      (Windows)
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Run Application
python run.py

Open browser:

http://127.0.0.1:5000
🗃 Database Schema Overview
Student Table

id

name

email

password

category

income

percentage

state

course_level

Scholarship Table

id

name

provider

category

income_limit

min_percentage

state

deadline

📊 Future Enhancements

🔍 AI-based recommendation scoring

📱 Mobile responsive enhancement

📧 Email deadline reminders

📄 Direct application link integration

🔐 OAuth Login (Google)

☁ Cloud deployment (Render / AWS)

🎯 Project Objectives

Improve scholarship accessibility

Reduce manual searching time

Increase application success rate

Promote transparency in eligibility filtering

🛡 Security Considerations

Password hashing

Input validation

Role-based authentication

Secure configuration management
