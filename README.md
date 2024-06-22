# Project Documentation: Applicant Tracking System (ATS) with Data Visualization

## Table of Contents

1. [Introduction](#1-introduction)
2. [Project Scope](#2-project-scope)
3. [Technologies Used](#3-technologies-used)
4. [System Architecture](#4-system-architecture)
5. [Setup and Installation](#5-setup-and-installation)
6. [Backend Development](#6-backend-development)
   - 6.1 [Django Setup](#61-django-setup)
   - 6.2 [Database Design](#62-database-design)
   - 6.3 [API Development](#63-api-development)
   - 6.4 [CV Parsing with Machine Learning](#64-cv-parsing-with-machine-learning)
7. [Frontend Development](#7-frontend-development)
   - 7.1 [Vue.js Setup](#71-vuejs-setup)
   - 7.2 [Dashboard Components](#72-dashboard-components)
   - 7.3 [Integration with Backend APIs](#73-integration-with-backend-apis)
   - 7.4 [Data Visualization](#74-data-visualization)
8. [Testing](#8-testing)
9. [Deployment](#9-deployment)
10. [Maintenance and Support](#10-maintenance-and-support)
11. [Conclusion](#11-conclusion)

---

## 1. Introduction

The Applicant Tracking System (ATS) project aims to streamline the recruitment process by automating candidate management, enhancing data-driven decision-making through machine learning, and providing insightful data visualization capabilities.

---

## 2. Project Scope

The project encompasses the following key features:

- **CV Parsing:** Utilizing machine learning for extracting and parsing candidate information from resumes (PDF, Word).
  
- **Candidate Matching:** Employing ML models to match candidates to job descriptions based on skills and qualifications.
  
- **Analytics Dashboard:** Visualizing recruitment metrics, candidate pipeline, and hiring trends through interactive data visualizations.

---

## 3. Technologies Used

- **Backend:** Django, Django REST Framework, Python
- **Frontend:** Vue.js, Vuex, JavaScript, HTML/CSS
- **Database:** PostgreSQL, MySQL
- **Machine Learning:** Python libraries (spaCy, scikit-learn)
- **Data Visualization:** Chart.js, D3.js
- **Deployment:** Docker, AWS, Heroku

---

## 4. System Architecture

### Overview

The system architecture is designed to ensure scalability, modularity, and seamless integration between backend and frontend components.

- **Backend:** Django serves as the core backend framework, handling data storage, APIs, and machine learning integration.
  
- **Frontend:** Vue.js provides a responsive and interactive user interface for managing candidates, jobs, and visualizing analytics.

### Components

- **Django Backend:**
  - **API Layer:** Django REST Framework for building RESTful APIs.
  - **Database:** PostgreSQL or MySQL for storing applicant data, job postings, and ML model outputs.
  
- **Vue.js Frontend:**
  - **Dashboard:** Components for displaying charts, tables, and metrics.
  - **Integration:** Axios for communicating with Django backend APIs.

---

## 5. Setup and Installation

### Prerequisites

- Python 3.x, pip, Node.js, npm
- IDE (e.g., VS Code)
- Docker (optional for deployment)

### Steps

1. **Backend Setup:**
   - Clone the repository and navigate to the backend directory.
   - Install dependencies: `pip install django djangorestframework django-cors-headers python-docx PyMuPDF`.
   - Configure database settings in `settings.py`.

2. **Frontend Setup:**
   - Initialize a new Vue.js project: `vue create frontend`.
   - Install Axios for API communication: `npm install axios`.

3. **Integration:**
   - Configure Axios to communicate with Django backend APIs in Vue.js (`main.js`).

---

## 6. Backend Development

### 6.1 Django Setup

#### Project Initialization

```bash
django-admin startproject your_project_name
cd your_project_name
python manage.py startapp api
